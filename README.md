# pye-community-bot

Discord moderation and utility bot for the **PyE Community** server.

[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](./LICENSE)

## Features
- Community utility commands
- Translation helpers
- Optional AI integrations (Cohere / HuggingFace)
- TypeScript-first codebase with lint + type checks

## Tech stack
- Node.js + TypeScript
- discord.js v14
- ESLint + commitlint + husky

## Getting started

### 1) Install dependencies
```bash
pnpm install
```

### 2) Configure environment
```bash
cp .env.example .env
```

Required variables:
- `DISCORD_TOKEN`
- `CLIENT_ID`
- `GUILD_ID`

Optional variables:
- `COHERE_AI_API_KEY`
- `HF_SECRET`

### 3) Run locally
```bash
pnpm run dev
```

### 4) Production run
```bash
pnpm run start
```

## Quality checks
```bash
pnpm run typecheck
pnpm run lint
pnpm run build
```

## Roadmap
Portfolio roadmap is maintained in [`ROADMAP.md`](./ROADMAP.md).

## Contributing
Contributions are welcome. Open an issue to discuss substantial changes before submitting a PR.

## License
MIT
