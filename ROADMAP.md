# ROADMAP

## Quick wins
- Add `.env.example` with required and optional provider keys.
- Harden README with clear setup, scripts, and deployment notes.
- Add `CONTRIBUTING.md` and PR quality checklist.
- Add healthcheck command to validate env + startup prerequisites.

## Medium
- Add unit tests for command handlers and service adapters.
- Introduce CI workflow (lint + typecheck + build).
- Add structured logging and error boundaries for external AI providers.
- Add command permission matrix and moderation safety notes.

## Big bets
- Modular plugin architecture for commands/events.
- Multi-provider fallback strategy with observability metrics.
- Staging bot profile with sandbox guild integration tests.

## Strategic rewrites
- Move to layered architecture (core domain + adapters + transport).
- Split infra/config into typed runtime schema with strict validation.
- Add contract tests for Discord API interactions and provider responses.
