# 3com Architecture

Status: draft, pending PRD
Last updated: 2026-09-11

This document fixes the technical foundation so that product work can start
the moment the PRD lands. Everything that depends on the PRD is marked as
`TBD (PRD)` rather than guessed.

## 1. Scope

Two user-facing surfaces plus one shared backend:

| Surface | Purpose | Stack |
|---|---|---|
| Mobile app | The product. Tracking, training, everything a user does. | Expo / React Native, TypeScript |
| Website | Marketing landing page. Positioning, waitlist, store links, legal. | Next.js (static export), TypeScript |
| Backend | Auth, data, sync, files. | Supabase (Postgres + Auth + Storage + Edge Functions) |

Out of scope for v1: web app with login, Apple Watch / Wear OS companion,
offline-first conflict resolution beyond simple last-write-wins.

## 2. Repository layout

A pnpm workspace monorepo. One repo, one install, shared types between app
and site.

```
3com/
├── apps/
│   ├── mobile/              # Expo app (iOS + Android)
│   └── web/                 # Next.js marketing site
├── packages/
│   ├── core/                # Domain model, types, validation, pure logic
│   ├── api/                 # Generated Supabase types + typed data access
│   └── config/              # Shared eslint / tsconfig / prettier presets
├── supabase/
│   ├── migrations/          # SQL migrations, source of truth for the schema
│   └── functions/           # Edge functions
└── docs/
    ├── PRD.md
    ├── ARCHITECTURE.md
    └── adr/                 # Architecture decision records
```

Rule: business logic lives in `packages/core` and is framework-free. Apps
render it, they do not own it. This is what makes a later web app cheap.

## 3. Stack decisions in brief

Full reasoning in `docs/adr/`.

- **pnpm + Turborepo** for the workspace. Fast, standard, good caching.
- **Expo (managed workflow)** for mobile. One codebase for iOS and Android,
  OTA updates via EAS Update, no Xcode needed for day-to-day work.
- **Expo Router** for navigation. File-based, same mental model as Next.js.
- **Next.js, static export** for the marketing site. Deploys anywhere, no
  server needed for a landing page, good SEO.
- **Supabase** for the backend. Postgres with row level security means auth
  and authorisation are one mechanism, not two. Self-hostable if needed.
- **TypeScript strict everywhere.** No JavaScript files in the workspace.
- **Zod** for schema validation, shared between client and edge functions.
- **TanStack Query** for server state in the app, **Zustand** for the little
  local UI state that is left.

## 4. Data model

`TBD (PRD)`. The entities below are the minimum any fitness tracker needs
and are safe to assume. The PRD decides everything beyond that.

```
users        id, created_at, display_name, locale, units (metric|imperial)
activities   id, user_id, type, started_at, duration_s, distance_m, source
metrics      id, activity_id, key, value, unit        # HR, pace, power, ...
```

Open questions the PRD has to answer:
- Which activity types, and is the set fixed or user-extensible?
- Is there a social layer (friends, groups, feeds)? That changes RLS a lot.
- Do we ingest from Apple Health / Google Health Connect / Garmin / Strava,
  or is manual and in-app recording enough for v1?
- Is there a paid tier? That decides whether we need billing from day one.

## 5. Non-functional baseline

- **Privacy.** Health data is a special category under GDPR Art. 9. Data
  stays in the EU region, no third-party analytics SDK in the app without an
  explicit decision, and a data export plus account deletion path ships with
  v1, not after it.
- **Offline.** The app must record an activity without network and sync
  later. Queue writes locally, reconcile on reconnect.
- **Testing.** Unit tests on `packages/core` (Vitest), component tests on the
  app (React Native Testing Library), one end-to-end smoke path (Maestro).
- **CI.** GitHub Actions: typecheck, lint, test on every push. EAS build on
  tags.

## 6. Environments

| Env | Supabase project | App | Web |
|---|---|---|---|
| local | local Supabase CLI stack | Expo Go / dev client | `next dev` |
| staging | separate project | EAS internal distribution | preview deploy |
| production | separate project | App Store / Play Store | production domain |

Secrets never live in the repo. App config comes from `app.config.ts` reading
`EXPO_PUBLIC_*` variables, web config from `.env.local`.

## 7. Delivery sequence

1. Workspace scaffold: pnpm, Turborepo, shared configs, CI. Product-agnostic.
2. Marketing landing page. Can ship before the app exists and starts the
   waitlist.
3. Supabase schema plus auth flow in the app.
4. Core tracking loop from the PRD.
5. Everything else, PRD order.

Step 1 and 2 do not need the PRD. Step 3 onward does.
