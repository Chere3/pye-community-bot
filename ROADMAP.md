# ROADMAP

This roadmap keeps the project active, contributor-ready, and production-minded.

## Quick wins (1-2 PRs)
- Add CI pipeline for `pnpm lint` + `pnpm typecheck` on pull requests.
- Add `.env.example` and stricter startup validation for optional provider keys.
- Expand command help output with category grouping and usage examples.
- Add basic unit tests for utility functions (`src/utils/text.ts`).

## Medium (next 2-4 weeks)
- Move hardcoded channel/user IDs from `src/config.ts` to structured runtime config files.
- Add command-level permission middleware for owner/developer/admin roles.
- Introduce centralized logger with severity levels and trace IDs for moderation events.
- Add anti-spam/rate-limit protections for high-traffic message handlers.

## Big bets (quarter)
- Split monolithic bot logic into modular feature packages (`commands`, `events`, `services`).
- Add persistence layer (SQLite/Postgres) for moderation history and bot telemetry.
- Add integration tests for Discord interactions using mocked gateway events.
- Design multilingual UX for command responses and moderation notices.

## Strategic rewrites (as needed)
- Refactor to domain-driven architecture: platform adapters (Discord), application services, and infra boundaries.
- Introduce typed config schema validation (`zod`/`envalid`) with environment-specific profiles.
- Replace ad-hoc event handling with a unified event bus + error boundary strategy.
- Build an observability baseline (structured logs, error reporting, uptime checks, dashboard).
