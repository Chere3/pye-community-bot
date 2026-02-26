# PyE Community Bot

Community Discord bot for [discord.gg/programacion](https://discord.com/invite/programacion), focused on practical utilities and AI-assisted interactions.

## Project quality goals
- Clear onboarding for contributors
- Predictable local setup and scripts
- Portfolio-ready docs and roadmap

See also:
- [ROADMAP.md](./ROADMAP.md)
- [CONTRIBUTING.md](./CONTRIBUTING.md)

## Tech stack
- TypeScript
- Discord.js v14
- pnpm
- ESLint + TypeScript checks

## Quick start
1. Install dependencies
   ```bash
   pnpm install
   ```
2. Create env file
   ```bash
   cp .env.example .env
   ```
3. Fill required values in `.env`
4. Run in development
   ```bash
   pnpm dev
   ```

## Production run
```bash
pnpm start
```

## Scripts
- `pnpm dev` — run bot in development mode
- `pnpm lint` — lint source files
- `pnpm typecheck` — TypeScript validation
- `pnpm build` — compile to `build/`
- `pnpm start` — typecheck + lint + build + run

## Environment variables
Required:
- `DISCORD_TOKEN`
- `CLIENT_ID`
- `GUILD_ID`

Optional:
- `COHERE_AI_API_KEY`
- `HF_SECRET`

## Validation checklist
Before opening a PR:
```bash
pnpm lint
pnpm typecheck
pnpm build
```

## License
MIT
