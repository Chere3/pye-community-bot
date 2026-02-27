# ROADMAP

## Quick wins (1-2 weeks)
- Add CI workflow for `pnpm lint` + `pnpm typecheck` + `pnpm build`.
- Add command-level docs (purpose, required permissions, examples).
- Introduce issue/PR templates for contributor consistency.
- Add structured logging format for command execution and failures.

## Medium initiatives (1-2 months)
- Add integration tests for slash command registration and handler routing.
- Introduce typed configuration validation (zod/envalid) for runtime safety.
- Add observability hooks (error reporting + basic command metrics).
- Improve i18n workflow for Spanish/English responses.

## Big bets (quarter)
- Migrate command architecture to plugin system (modular command packs).
- Add persistence layer for moderation, preferences, and feature flags.
- Build admin dashboard for bot health and command usage analytics.

## Strategic rewrites
- Move to event-driven domain modules with explicit contracts between bot core and feature modules.
- Separate deployment/runtime concerns into a standalone package (monorepo split).
- Replace ad-hoc AI integration with provider abstraction and safety policies.
