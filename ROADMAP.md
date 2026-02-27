# ROADMAP

## Quick wins (1-2 weeks)
- Add `.env.example` and setup guardrails for first-time contributors.
- Improve README with explicit local run, lint, and typecheck flow.
- Add CONTRIBUTING guidelines and issue/PR expectations.
- Document required bot permissions and basic troubleshooting.

## Medium improvements (2-6 weeks)
- Add CI (lint + typecheck + build) on pull requests.
- Add command registry docs to map each feature to source files.
- Improve config validation at startup for missing env vars.

## Big bets (1-2 quarters)
- Refactor command/event loading into modular plugin architecture.
- Add observability (structured logs + error reporting).
- Introduce test harness for command handlers and utility services.

## Strategic rewrites (as needed)
- Migrate to layered architecture (`core`, `features`, `infra`) for maintainability.
- Introduce runtime feature flags for gradual rollout of experimental commands.
