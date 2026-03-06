# PyE Community - README

[![Discord](https://img.shields.io/discord/768278151435386900?color=7289da&label=Join%20Us%20on%20Discord&logo=discord&logoColor=white)](https://discord.gg/programacion)
[![GitHub](https://img.shields.io/github/license/pye-community/pye-community-bot)](https://github.com/pye-community/pye-community-bot)

Welcome to the PyE Community! Our Discord bot is designed to enhance your experience on [discord.gg/programacion](https://discord.com/invite/programacion) by providing valuable features and assistance to our members.

## Getting Started

Follow these simple steps to run the PyE Community bot on your server:

1. **Install Dependencies:** We recommend using [pnpm](https://pnpm.js.org/) as the package manager for this project. Install dependencies with your preferred package manager:

   ```bash
   pnpm install
   ```

2. **Create a Configuration File:** In the root directory of the project, create a `.env` file and provide the following details:

   ```env
   DISCORD_TOKEN=
   CLIENT_ID=
   GUILD_ID=
   COHERE_AI_API_KEY=    # (optional)
   HF_SECRET=            # (optional)
   ```

3. **Start the Bot:** Run the following command to start the bot:

   ```bash
   pnpm run start
   ```

## Contributing

We value contributions from our community members. If you have any ideas or improvements, please open an issue to discuss them before submitting a pull request.

## License

This project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/). Feel free to use and modify it according to your needs.

---

## Scripts

- `pnpm dev` - run bot in watch mode
- `pnpm build` - compile TypeScript to `build/`
- `pnpm start` - lint + typecheck + build + run
- `pnpm ci` - local CI parity checks

## Architecture overview

- `src/events/` event-driven Discord handlers
- `src/commands/` slash and utility commands
- `src/modules/` shared helpers and handler loading
- `src/config.ts` validated runtime configuration
