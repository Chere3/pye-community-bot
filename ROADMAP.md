# ROADMAP

## Quick wins
- [ ] Add GitHub Actions CI for lint/typecheck/build on PRs.
- [ ] Add command inventory documentation under `docs/commands.md`.
- [ ] Add structured `.env.example` and startup validation errors.
- [ ] Introduce logger abstraction for production troubleshooting.

## Medium
- [ ] Add modular command loading + per-command cooldown configuration.
- [ ] Add role-based permission middleware for admin commands.
- [ ] Add test suite for command handlers and utility modules.
- [ ] Add telemetry hooks (error rate, command usage heatmap).

## Big bets
- [ ] Migrate to slash-command-first architecture with dynamic registration.
- [ ] Add localization layer for ES/EN responses.
- [ ] Add anti-spam and moderation automations with configurable policies.

## Strategic rewrites
- [ ] Split into packages (`core`, `commands`, `integrations`) for long-term maintainability.
- [ ] Evaluate queue-based worker model for heavy AI requests.
