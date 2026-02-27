# PyE Community Bot

[![Discord](https://img.shields.io/discord/768278151435386900?color=7289da&label=Join%20Us%20on%20Discord&logo=discord&logoColor=white)](https://discord.gg/programacion)
[![GitHub](https://img.shields.io/github/license/pye-community/pye-community-bot)](https://github.com/pye-community/pye-community-bot)

Discord bot for the PyE community server: <https://discord.gg/programacion>.

## Quickstart

```bash
pnpm install
cp .env.example .env
pnpm start
```

## Environment variables

Required:
- `DISCORD_TOKEN`
- `CLIENT_ID`
- `GUILD_ID`

Optional:
- `COHERE_AI_API_KEY`
- `HF_SECRET`

See `.env.example` for template values.

## Development commands

- `pnpm dev` — start in watch mode
- `pnpm lint` — run ESLint
- `pnpm typecheck` — run TypeScript checks
- `pnpm build` — compile to `build/`
- `pnpm start` — run full quality gate + build + bot startup

## Project standards

- Contribution workflow: [CONTRIBUTING.md](./CONTRIBUTING.md)
- Portfolio roadmap and planned refactors: [ROADMAP.md](./ROADMAP.md)

## License

Licensed under the [MIT License](https://choosealicense.com/licenses/mit/).
