# PyE Community Bot

Discord bot for the PyE community server (`discord.gg/programacion`) focused on moderation support, utility flows, and community automation.

## Tech stack
- Node.js + TypeScript
- discord.js v14
- pnpm

## Project structure
- `src/events/` → Discord event handlers
- `src/modules/` → command and helper modules
- `src/config.ts` → environment-driven configuration
- `src/index.ts` → startup and runtime wiring

## Quick start
### 1) Install
```bash
pnpm install
```

### 2) Configure
Copy `.env.example` to `.env` and fill required values:
```bash
cp .env.example .env
```

### 3) Run locally
```bash
pnpm run dev
```

### 4) Build and run production mode
```bash
pnpm run build
pnpm run start
```

## Quality commands
```bash
pnpm run lint
pnpm run typecheck
pnpm run build
pnpm run validate
```

## CI
GitHub Actions runs lint, typecheck, and build on pull requests and pushes to `main`.

## Operational checklist
- Verify bot token and app IDs are present in `.env`.
- Ensure bot intents enabled in Discord Developer Portal.
- Re-register slash commands when command definitions change.

## Contributing
1. Create a feature branch.
2. Keep PRs scoped to one improvement area.
3. Run `pnpm run validate` before opening PR.
4. Include rollout/verification notes in the PR description.

## License
MIT
