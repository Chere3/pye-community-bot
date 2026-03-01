# ROADMAP

## Quick wins (0-4 weeks)
- Add `.env.example` with required/optional environment variables and comments.
- Add CI pipeline for lint + typecheck + build on push/PR.
- Expand README with architecture overview and runbook commands.
- Add health and troubleshooting section for common Discord bot startup failures.

## Medium-term improvements (1-2 months)
- Introduce command/event test harness with mocked Discord client.
- Add structured logging with correlation IDs for moderation/action traces.
- Add rate-limit and retry wrappers for external AI providers.
- Add configuration validation (schema-based) at boot.

## Big bets (1-2 quarters)
- Modularize bot into domain packages (events, commands, integrations) for maintainability.
- Add observability stack (metrics + uptime + alerting).
- Build staged deployment strategy (dev/staging/prod guilds).

## Strategic rewrites
- Replace ad-hoc loading with a plugin architecture for commands and events.
- Move to fully typed configuration contracts and dependency injection.
- Introduce message-processing pipeline for moderation, AI, and analytics extensions.
