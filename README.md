# PyE Community Bot

[![Discord](https://img.shields.io/discord/768278151435386900?color=7289da&label=Join%20Us%20on%20Discord&logo=discord&logoColor=white)](https://discord.gg/programacion)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](./LICENSE)

A TypeScript Discord bot focused on community support and moderation utilities for **discord.gg/programacion**.

## Features
- Slash-command support (utility + developer commands)
- Event-driven Discord handlers (`ready`, `messageCreate`, `interactionCreate`, `threadCreate`)
- Community helper modules (reporting + thread sharing)
- Optional AI integrations (Cohere + Hugging Face) for moderation/analysis workflows

## Project structure

```txt
src/
  commands/        # Slash commands (utility, developer)
  events/          # Discord event listeners
  modules/         # Domain-specific helpers and bot modules
  utils/           # Shared helpers
  config.ts        # Runtime config + env checks
  index.ts         # App entrypoint
```

## Prerequisites
- Node.js 20+
- pnpm 8+
- Discord application + bot token

## Setup

```bash
pnpm install
cp .env.example .env
```

Fill required environment variables in `.env`:

| Variable | Required | Description |
| --- | --- | --- |
| `DISCORD_TOKEN` | Yes | Bot token from Discord Developer Portal |
| `CLIENT_ID` | Yes | Discord application client ID |
| `GUILD_ID` | Yes | Target Discord server ID |
| `COHERE_AI_API_KEY` | No | Optional Cohere integration key |
| `HF_SECRET` | No | Optional Hugging Face API token |

## Scripts

| Script | Command | Purpose |
| --- | --- | --- |
| `dev` | `pnpm dev` | Run with hot reload in development |
| `start` | `pnpm start` | Typecheck, lint, build, then run |
| `build` | `pnpm build` | Compile TypeScript to `build/` |
| `lint` | `pnpm lint` | Run ESLint |
| `lint:fix` | `pnpm lint:fix` | Auto-fix lint issues |
| `typecheck` | `pnpm typecheck` | Validate TypeScript types |
| `clean` | `pnpm clean` | Remove build artifacts |

## Development workflow
1. Create a feature branch from `main`.
2. Run `pnpm dev` while iterating.
3. Before opening a PR, run:

```bash
pnpm lint
pnpm typecheck
pnpm build
```

4. Open PR with scope, risks, and validation notes.

## Contributing
See [CONTRIBUTING.md](./CONTRIBUTING.md) for commit style, branch naming, and PR checklist.

## Roadmap
See [ROADMAP.md](./ROADMAP.md) for short, medium, and strategic priorities.

## License
MIT — see [LICENSE](./LICENSE).
