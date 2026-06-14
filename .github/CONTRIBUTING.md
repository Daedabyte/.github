# Contributing (Daedabyte repos)

## Branch model
`feature/* → staging (default) → main (production, Amplify deploy)`
- Feature branches: `<type>/<slug>` (`fix/…`, `chore/…`). Squash-merged.
- `staging` is the default and integration branch; PRs target it.
- `main` is production; promote via PR only. **Never `git push origin main`.**

## CI gate (required, no bypass)
Every PR into `staging`/`main` must pass `typecheck`, `lint`, `format`, `build`.
0 approvals required, but the checks cannot be bypassed — including your own PRs.

## Merging
Squash-only into `staging`; `staging → main` promotions merge as a merge commit. The
repo auto-deletes the branch on merge. Use `gh pr merge --squash` (or `--merge` for a
promotion).
