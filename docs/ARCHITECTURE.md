# Architecture Overview

## High-level flow
1. `src/index.ts` boots the Discord client and logs in using validated config.
2. Bot event handlers are initialized from `src/modules/bot/handlers.ts`.
3. Commands/events are routed into module functions under `src/modules/bot/functions`.
4. Optional AI features are enabled when provider keys are present.

## Source layout
- `src/index.ts` — app entrypoint and startup lifecycle.
- `src/config.ts` — environment loading + required variable validation.
- `src/modules/bot/handlers.ts` — Discord event wiring and command registration.
- `src/modules/bot/functions/*` — command logic and feature handlers.

## Configuration boundaries
- Runtime configuration is centralized in `src/config.ts`.
- Required vars: `CLIENT_ID`, `DISCORD_TOKEN`, `GUILD_ID`.
- Optional vars enable integrations (for example `COHERE_AI_API_KEY`).

## Design intent
- Keep transport concerns (Discord events) separate from feature logic.
- Keep command handlers small and delegate logic to dedicated modules.
- Prefer explicit validation on startup to fail fast on invalid config.
