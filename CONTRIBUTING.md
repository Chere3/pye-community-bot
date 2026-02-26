# Contributing

## Branching
- Base branch: `main`
- Branch naming:
  - `feat/...` for features
  - `fix/...` for bug fixes
  - `chore/...` for maintenance/docs/infra

## Commit format
Use Conventional Commits:
- `feat: ...`
- `fix: ...`
- `docs: ...`
- `chore: ...`

## Pull request checklist
- [ ] Problem statement and scope are clear
- [ ] `pnpm lint` passes
- [ ] `pnpm typecheck` passes
- [ ] `pnpm build` passes
- [ ] README/docs updated when behavior changes
- [ ] New env vars documented in `.env.example`

## Coding guidelines
- Keep bot logic modular and testable.
- Avoid hardcoding secrets/config in source files.
- Add explicit error handling for API-dependent flows.
- Keep user-facing messages concise and safe.
