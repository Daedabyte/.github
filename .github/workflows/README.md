# Reusable workflows (org-wide)

This directory hosts **reusable** GitHub Actions workflows other Daedabyte repos call:
`uses: Daedabyte/.github/.github/workflows/<file>.yml@<ref>`.

- `astro-ci.yml` — the shared typecheck/lint/format/build pipeline for Astro sites.

NOTE: a workflow placed here runs ONLY for this repo unless it is `on: workflow_call`
and explicitly invoked by another repo. If this repo is private, callers also require
org Actions access to be enabled (Settings → Actions → "Accessible from repositories in
the organization") before they can `uses:` these workflows.
