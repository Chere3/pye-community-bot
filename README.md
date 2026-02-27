# PyE Community Bot

[![Discord](https://img.shields.io/discord/768278151435386900?color=7289da&label=Join%20Us%20on%20Discord&logo=discord&logoColor=white)](https://discord.gg/programacion)
[![License](https://img.shields.io/github/license/Chere3/pye-community-bot)](./LICENSE)

Discord bot for the **PyE Community** server, focused on automation, moderation support, and community interaction helpers.

## Features
- Slash-command based interaction flow.
- Centralized startup configuration validation.
- Modular handler/function structure under `src/modules/bot`.
- Optional AI-powered features (when API keys are present).

## Architecture at a glance
- `src/index.ts`: startup and Discord client lifecycle.
- `src/config.ts`: environment loading and required variable checks.
- `src/modules/bot/handlers.ts`: event wiring + command registration.
- `src/modules/bot/functions/*`: command/business logic.

Detailed module notes: [`docs/ARCHITECTURE.md`](./docs/ARCHITECTURE.md)

## Prerequisites
- Node.js 20+
- pnpm 8+
- Discord application + bot token

## Installation
```bash
pnpm install
cp .env.example .env
```

## Environment variables
Required:
- `CLIENT_ID`
- `DISCORD_TOKEN`
- `GUILD_ID`

Optional:
- `COHERE_AI_API_KEY`

See `.env.example` for placeholders.

## Development workflow
```bash
pnpm dev
```

## Scripts
- `pnpm start`: typecheck + lint + build + run.
- `pnpm dev`: local dev loop with auto-restart.
- `pnpm lint`: lint TypeScript source.
- `pnpm typecheck`: run TypeScript compiler checks.
- `pnpm build`: compile TS to `build/`.
- `pnpm clean`: remove build output.

## Quality checks
Recommended before every PR:
```bash
pnpm lint
pnpm typecheck
pnpm build
```

## Project management
- Contribution guide: [`CONTRIBUTING.md`](./CONTRIBUTING.md)
- Portfolio roadmap: [`ROADMAP.md`](./ROADMAP.md)

## Release and maintenance notes
- Keep dependencies updated in small, reviewable batches.
- Validate startup configuration on every environment change.
- Prefer small scoped PRs with explicit validation notes.

## License
MIT — see [`LICENSE`](./LICENSE).
