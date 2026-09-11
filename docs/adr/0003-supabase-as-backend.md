# ADR 0003: Supabase as the backend

Date: 2026-09-11
Status: proposed

## Context

The app needs authentication, a database, file storage for media, and a place
to run server-side logic. The data is health data, which is a special
category under GDPR Art. 9, so residency and deletion paths matter.

Options considered:

1. **Supabase.** Managed Postgres with row level security, auth, storage and
   edge functions. EU regions available. Self-hostable, so no hard lock-in.
2. **Firebase.** Very fast to start, excellent offline SDK. Document model
   makes the aggregate queries a tracking app needs (weekly volume, trends,
   leaderboards) awkward, and data residency is less clean for EU health data.
3. **Own backend (NestJS or Go plus managed Postgres).** Full control, most
   work. Not justified before the PRD proves something Supabase cannot do.

## Decision

Supabase, EU region. The schema is owned by SQL migrations in
`supabase/migrations`, not by the dashboard. Authorisation is expressed as
row level security policies, so the same rules apply to every client.

## Consequences

- Postgres means real SQL for trend and aggregate queries, which a fitness
  tracker needs constantly.
- RLS is the single place authorisation lives. It also means every new table
  needs a policy, and a table without one is a leak. Migrations must be
  reviewed with that in mind.
- Offline support is not built in the way Firebase offers it. The app needs
  its own local write queue. Planned in the architecture doc.
- Status stays *proposed* until the PRD confirms there is no requirement
  (real-time multiplayer at scale, heavy ML serving) that changes the answer.
