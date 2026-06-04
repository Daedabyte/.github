# Reusable workflows (org-wide)

This directory hosts **reusable** GitHub Actions workflows other Daedabyte repos call:
`uses: Daedabyte/.github/.github/workflows/<file>.yml@main`.

Planned (see github-optimization roadmap):
- `astro-ci.yml` — item #1: the shared typecheck/lint/format/build pipeline.
- `dependabot-automerge.yml` — item #2: tiered Dependabot auto-merge to `staging`.

NOTE: a workflow placed here runs ONLY for this repo unless it is `on: workflow_call`
and explicitly invoked by another repo. Because this repo is **private**, private callers
require org Actions access to be enabled (Settings → Actions → "Accessible from
repositories in the organization") before they can `uses:` these workflows.
