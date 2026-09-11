# 05 Product and MVP Specification

Language: English (build documentation).

## MVP thesis

Ship exactly one loop, end to end, done well:

> **Post a session -> get discovered by the right people -> they join -> it happens -> a trace
> of it stays visible.**

Everything not in that loop is out of scope for v1, no matter how obvious it seems.

## Scope decision

The chosen path is a custom PWA from the start (no zero-code detour). The corresponding risk is
that the product ships into an empty room. Mitigation is not a different product, it is
sequencing: **the rituals start in week 1, the PWA lands in week 8 to 10.** See `07-go-to-market.md`.

A PWA (not native) because:
- One codebase, installable on iOS and Android home screens
- No app store review cycle, ship daily
- The core use case is planning and browsing, not background GPS tracking
- Push notifications work on iOS PWAs since iOS 16.4 (verify current behaviour before relying on it)

Native becomes relevant only if push reliability or Strava live integration proves limiting.

## v1 feature scope

### In scope

**Onboarding and profile**
- Sign in with email magic link or Strava OAuth
- Profile: name, photo, home district, disciplines, target race and date, self-declared level per discipline
- Pace and power bands per discipline, self-declared, with a plain-language scale:
  - Swim: min/100m band (e.g. 1:35 to 1:50)
  - Bike: watts/kg band or plain speed band on flat
  - Run: min/km band at easy pace and at threshold
- Optional Strava connection to prefill bands from recent activities (strong trust signal, do it if cheap)

**Session board (the core)**
- Create a session: discipline, date/time, meeting point (map pin + text), session type, intensity, pace band, capacity, visibility, note
- Browse: list and map view, filtered by discipline, day, district, pace band overlap
- **Pace fit indicator:** each session shows "fits you", "slightly fast", "slightly slow", "outside your band" against the viewer's declared band. This is the single most important UI element in the product.
- Join, leave, waitlist
- Host can approve requests when the session is set to "on request"
- Recurring sessions (weekly), because the anchor rituals live here

**Session lifecycle**
- Automatic reminder 12 hours before
- Host can cancel with a reason, participants get notified
- After the session: one-tap "we were there" with optional photo and short text -> becomes a feed post

**Feed (deliberately thin)**
- Posts from completed sessions only, plus host announcements
- Kudos and comments
- No automatic activity import, no leaderboards, no segments

**Notifications**
- Someone joined your session
- A session matching your bands and district was posted (max 1 digest per day)
- Reminder before a session you joined
- Session cancelled

**Trust and safety**
- Real name and photo required
- Report and block
- Community guidelines accepted at signup, including an explicit "this is not a dating platform" clause
- Liability disclaimer at session join: participation at own risk, everyone is responsible for their own equipment, insurance and fitness

**Admin (you)**
- Create curated sessions and brand events
- Feature a session on top of the board
- Basic dashboard: users, sessions created, join rate, show-up rate, repeat rate

### Explicitly out of scope for v1

- Payments in-app (use an external link: bank transfer, PayPal, Eversports, whatever the studio uses)
- Direct messaging between users (group chat per session only, or a WhatsApp link posted by the host)
- Training plans, workout structure, FTP, TSS
- Coach profiles and search
- Multi-city support in the UI (build the data model city-aware, hide the switcher)
- Gamification beyond a simple group streak
- Web content, blog, SEO pages
- Native apps

Direct messaging is the most tempting cut to reverse. Resist it in v1: 1:1 DMs in a
mixed-gender sports community create moderation load you cannot carry alone, and per-session
group chat covers the actual coordination need.

## Key user stories

| # | As a | I want to | So that | Priority |
|---|---|---|---|---|
| 1 | age-grouper | post the long ride I already planned for Saturday | I do not have to ride 4 hours alone | P0 |
| 2 | age-grouper | see at a glance whether a session fits my pace | I do not embarrass myself or ruin my session | P0 |
| 3 | beginner | join a session led by someone experienced | I learn without paying for coaching | P0 |
| 4 | host | see who is coming and cancel if nobody is | I do not wait in the rain for nobody | P0 |
| 5 | member | get notified about sessions in my district and band | I do not have to check the app daily | P1 |
| 6 | member | post a photo after a session | the group stays visible and others want in | P1 |
| 7 | organiser (you) | run a recurring Saturday ride as a fixed anchor | there is always something on the board | P0 |
| 8 | organiser (you) | publish a coached track session with limited spots | the community gets quality it cannot self-organise | P1 |
| 9 | brand partner | run a testing event with a signup list | I reach athletes in the moment of use | P2 |

## Screens (v1)

1. **Board** (default): filter bar, list of upcoming sessions with pace-fit badge, floating "create" button
2. **Session detail**: all info, participants with their bands, join button, map, group chat thread
3. **Create session**: single scrolling form, smart defaults from the user's last session
4. **Feed**: post-session posts, kudos
5. **Profile**: own and others', bands, upcoming and past sessions, reliability indicator (share of joined sessions actually attended)
6. **Onboarding**: 4 steps, maximum 90 seconds

The reliability indicator matters more than it looks. No-shows are the fastest way to kill a
session board. Making attendance visible, without shaming, is the cheapest available mechanism.

## Definition of done for the MVP

Not "features complete". The MVP is done when, for four consecutive weeks:
- at least 10 sessions per week exist on the board,
- at least half of them were created by someone other than the founder,
- and the median session has 3 or more participants who actually showed up.
