# 06 Technical Architecture

Language: English (build documentation).

## Guiding constraint

One part-time builder. The stack must minimise operational work, not maximise elegance. Every
component that needs babysitting is a component that will kill the project in month 4.

## Recommended stack

| Layer | Choice | Rationale |
|---|---|---|
| Frontend | Next.js (App Router) + TypeScript + Tailwind + shadcn/ui | PWA-capable, fast to build, huge ecosystem, good AI-assisted development support |
| Backend and DB | Supabase (Postgres, Auth, Storage, Realtime, Row Level Security) | Auth, database, file storage and realtime in one managed product. RLS handles most authorisation without a backend layer. |
| Hosting | Vercel | Zero-config for Next.js, free tier sufficient at this scale |
| Maps | MapLibre + OpenStreetMap tiles, or Mapbox free tier | Meeting points are central to the product |
| Push | Web Push (VAPID) via service worker; verify current iOS PWA behaviour | Notifications drive the join loop |
| Transactional email | Resend or Postmark | Reminders and digests |
| Analytics | PostHog (self-serve tier) | Funnel analysis matters more than page views here |
| Error tracking | Sentry | |
| Payments (later) | Stripe | Out of scope for v1 |

Alternative worth considering if you want to move faster with AI tooling: the same Supabase
backend with a Vite + React SPA. Next.js is the safer long-term bet; the SPA is faster to
prototype. Decide once, do not migrate later.

## Data model (v1)

```
users
  id, created_at, display_name, photo_url, home_district, city_id,
  bio, target_race, target_race_date, strava_athlete_id, reliability_score

user_bands
  id, user_id, discipline (swim|bike|run|trail|strength),
  tempo_group (kaffeefahrt|tempo|vollgas),     -- what the user sees and picks
  band_low, band_high,                          -- numeric, never shown
  unit (sec_per_100m | watt_per_kg | sec_per_km | vertical_m_per_h | relative),
  source (self_declared | strava_derived), updated_at

  -- strength/Hyrox has no meaningful pace unit: use tempo_group alone with
  -- unit='relative'. Do not invent a metric to keep the schema symmetric.

cities
  id, name, slug, timezone, bounds        -- present from day one, hidden in UI

sessions
  id, host_user_id, city_id, title, description,
  discipline (swim|bike|run|trail|strength|brick|other),
  session_type (endurance|tempo|interval|long|recovery|brick|technique|race_sim|circuit),
  starts_at, duration_min,
  meeting_point_lat, meeting_point_lng, meeting_point_label, district,
  pace_band_low, pace_band_high, pace_band_unit,
  capacity, visibility (open|on_request|private),
  layer (peer|curated|brand),
  cost_cents, cost_note, external_booking_url,
  recurrence_rule, parent_session_id,
  status (scheduled|cancelled|completed), cancelled_reason,
  created_at

session_participants
  id, session_id, user_id,
  status (joined|waitlisted|requested|declined|cancelled),
  attended (null|true|false), joined_at

posts
  id, author_user_id, session_id (nullable), body, photo_urls[], created_at

kudos
  id, post_id, user_id, created_at

comments
  id, post_id, user_id, body, created_at

session_messages          -- per-session group chat
  id, session_id, user_id, body, created_at

partners                  -- brands, studios, coaches
  id, name, type (brand|studio|coach|shop), contact, notes, city_id

reports                   -- trust and safety
  id, reporter_user_id, target_user_id, target_session_id, reason, created_at, resolved
```

Notes:
- `city_id` on `sessions` and `users` from day one. Adding multi-city later to a single-city
  schema is the classic avoidable migration.
- `pace_band_*` stored as integers in a canonical unit per discipline (seconds per 100m,
  watts per kg times 100, seconds per km) to make overlap queries trivial.
- `attended` drives `reliability_score`. Set it by host confirmation plus self-confirmation.

## The pace-fit calculation

The single most important piece of logic. Keep it simple and explainable:

```
overlap = max(0, min(user_high, session_high) - max(user_low, session_low))
session_width = session_high - session_low

fit = overlap / session_width

fit >= 0.5   -> "passt zu dir"
0 < fit < 0.5 -> "knapp" (with direction: schneller / langsamer)
fit == 0 and user is faster  -> "für dich locker"
fit == 0 and user is slower  -> "ambitioniert für dich"
```

Never block a join based on fit. Inform, do not gate. Gating destroys the beginner funnel.

## Strava integration

Read-only, optional, OAuth. Two uses:

1. **Band prefill:** pull the last 90 days of activities, derive median easy pace per discipline,
   propose bands the user can adjust. Reduces onboarding friction and increases band accuracy.
2. **Session verification (later):** match a completed 3com session to a Strava activity to
   confirm attendance automatically.

Do not build a Strava feed mirror. Check Strava's API terms before any display of their data;
their terms restrict what can be shown and combined.

## Build plan

| Week | Deliverable |
|---|---|
| 1 | Schema, auth, onboarding, profile with bands |
| 2 to 3 | Session create and board with filters, pace-fit badge |
| 4 | Session detail, join and leave, capacity and waitlist |
| 5 | Notifications (email + web push), reminders |
| 6 | Post-session posts, feed, kudos |
| 7 | Recurring sessions, admin view, per-session chat |
| 8 | Trust and safety, guidelines, reporting, polish, closed beta |
| 9 to 10 | Beta feedback, bug fixing, public launch in Vienna |

Assumes roughly 10 to 15 hours per week with AI-assisted development. **[Hypothese]**

## Non-functional requirements

- Mobile-first, usable one-handed, readable outdoors at arm's length
- Board loads in under 1.5s on 4G
- German UI from day one, English as a second locale (Vienna has a large expat endurance scene)
- GDPR: location data of meeting points is fine, but never store user location traces.
  Data processing agreement with Supabase, privacy policy, deletion on request.
- Do not publish exact home addresses. Meeting points are public places only.
