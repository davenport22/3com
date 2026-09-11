# 3com

Sports and fitness tracking. Native app on iOS and Android, plus a marketing
website.

**Status:** pre-scaffold. Architecture is decided, the PRD is pending, no
application code yet.

## Documentation

| Document | What it holds |
|---|---|
| [docs/PRD.md](docs/PRD.md) | Product requirements. Currently a skeleton waiting to be filled. |
| [docs/ARCHITECTURE.md](docs/ARCHITECTURE.md) | Stack, repository layout, data model sketch, delivery sequence. |
| [docs/adr/](docs/adr/) | Architecture decision records, one file per expensive decision. |

## Planned stack

- **App:** Expo / React Native, Expo Router, TypeScript
- **Web:** Next.js, static export
- **Backend:** Supabase (Postgres, Auth, Storage, Edge Functions), EU region
- **Workspace:** pnpm workspaces with Turborepo

See [ADR 0002](docs/adr/0002-expo-and-nextjs-in-a-pnpm-monorepo.md) and
[ADR 0003](docs/adr/0003-supabase-as-backend.md) for the reasoning and the
alternatives that were rejected.

## Next steps

1. Fill the PRD.
2. Scaffold the pnpm workspace, shared configs and CI.
3. Build the marketing landing page. It does not depend on the PRD.
4. Supabase schema and auth, then the core tracking loop.
