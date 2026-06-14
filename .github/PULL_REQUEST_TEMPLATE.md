## What & why
<!-- One-line summary; link issue if any. -->

## Target branch
- [ ] `staging` (default — feature work integrates here first)
- [ ] `main` (production promotion only — triggers Amplify deploy)

## Checklist
- [ ] CI is green (`typecheck` · `lint` · `format` · `build`) — required, no bypass
- [ ] Squash merge (one commit per PR — repo default)
- [ ] For a `main` promotion: spot-checked affected pages (live Amplify deploy)
- [ ] Scope is minimal — touches only what the change needs

<!-- Reminder: never `git push origin main`; route through the PR flow. -->
