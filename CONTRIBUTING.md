# Contributing

Thanks for improving **pye-community-bot**.

## Branch naming
Use descriptive branch names:
- `feat/<scope>-<short-description>`
- `fix/<scope>-<short-description>`
- `chore/<scope>-<short-description>`

Examples:
- `feat/moderation-rate-limit`
- `chore/docs-professionalize-readme`

## Commit convention
This repository uses Conventional Commits.

Examples:
- `feat(commands): add welcome slash command`
- `fix(bot): handle missing guild permissions`
- `docs(readme): add architecture section`

## Local validation checklist
Before opening a PR, run:

```bash
pnpm install
pnpm lint
pnpm typecheck
pnpm build
```

If you changed runtime behavior, also run:

```bash
pnpm dev
```

## Pull request checklist
- [ ] Scope is focused and clearly described.
- [ ] Docs updated (`README.md`, `ROADMAP.md`, or module docs).
- [ ] Lint/typecheck/build pass locally.
- [ ] Environment changes reflected in `.env.example`.
- [ ] PR includes validation notes and potential risks.

## PR structure recommendation
Include these sections in your PR description:
1. **Summary**
2. **Changes made**
3. **Validation**
4. **Risk / rollback**
5. **Next steps**
