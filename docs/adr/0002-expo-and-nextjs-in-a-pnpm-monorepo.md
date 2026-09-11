# ADR 0002: Expo app and Next.js site in a pnpm monorepo

Date: 2026-09-11
Status: accepted

## Context

3com needs a native app on iOS and Android plus a marketing website. The
product logic behind both will overlap, at minimum in domain types and
validation. A future web app with login is plausible but not committed.

Options considered:

1. **Expo / React Native, monorepo with the web site.** One language, one
   toolchain, shared packages. Native modules occasionally need a custom dev
   client, which is routine but not free.
2. **Flutter app plus a separate web repo.** Excellent rendering performance
   and animation control. No code sharing with a React site, and a second
   language in the stack for a team that does not need one.
3. **PWA only.** Cheapest and no store review. Background location and
   continuous sensor access during a workout are unreliable on iOS, which is
   disqualifying for a tracking app.
4. **Native Swift first.** Best HealthKit and Watch integration, but doubles
   the effort for Android and blocks an Android launch behind a second build.

## Decision

Expo (managed workflow) with Expo Router for the app, Next.js with static
export for the marketing site, both in a pnpm workspace with Turborepo.
Shared domain code lives in `packages/core` and is framework-free.

## Consequences

- One TypeScript toolchain for everything. Lint, typecheck and test configs
  are written once in `packages/config`.
- EAS Build and EAS Update give builds and over-the-air JS updates without a
  local Xcode setup.
- Expensive native work (custom sensor handling, background tracking) needs a
  custom dev client. Budget a day the first time it comes up.
- If deep Apple Watch integration becomes a core requirement later, that is a
  separate native target, not a rewrite.
- A web app with login is later an additional `apps/` entry that reuses
  `packages/core`, not a new project.
