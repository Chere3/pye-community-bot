# Contributing to PyE Community Bot

Thanks for helping improve the bot.

## Workflow
1. Fork or create a branch from `main`.
2. Use branch names like:
   - `feat/<short-description>`
   - `fix/<short-description>`
   - `chore/<short-description>`
   - `docs/<short-description>`
3. Keep PRs scoped and focused.

## Commit convention
This repository uses Conventional Commits.

Examples:
- `feat(commands): add slash command cooldown middleware`
- `fix(events): guard missing thread parent`
- `docs(readme): add development setup`

## Local quality checks
Run before opening a PR:

```bash
pnpm install
pnpm lint
pnpm typecheck
pnpm build
```

## Pull request checklist
- [ ] Change is explained clearly in PR description.
- [ ] Related issue is linked (if available).
- [ ] Lint/typecheck/build pass locally.
- [ ] Added/updated docs when behavior changed.
- [ ] No secrets or environment tokens committed.

## Code style
- Keep TypeScript strict and explicit.
- Prefer small functions and clear naming.
- Avoid hidden side effects in command/event handlers.
