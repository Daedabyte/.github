# `Daedabyte/.github`

Org-meta repository. It serves two roles:

1. **Org-wide default community-health files.** GitHub auto-surfaces the files under
   `.github/` (PR template, issue forms, `SECURITY.md`, `CONTRIBUTING.md`) on **any
   Daedabyte repo that doesn't define its own** — fill-the-gap inheritance, not a copy.
2. **Reusable-workflow host.** `.github/workflows/` is where org-wide reusable GitHub
   Actions workflows live, called by member repos as
   `uses: Daedabyte/.github/.github/workflows/<file>.yml@<ref>` (note the doubled
   `.github/.github/`). The workflow bodies are added by the CI (#1) and Dependabot
   auto-merge (#2) roadmap items.

## Notes
- This repo is **private**, so `profile/README.md` (the public org landing card) is
  **dormant** — it only renders when the repo is public. It's seeded and ready if that
  changes.
- Reusable workflows hosted here are callable by private member repos **only if** org
  Actions access is enabled (Settings → Actions → "Accessible from repositories in the
  organization"). Owned by roadmap item #1.
- This repo is intentionally **outside** the `astro-site-protection` standard — it's not
  an Astro site, has no `astro-site` custom property, and runs none of the 4 CI checks.
  Do **not** tag it `astro-site=true` (it would self-lock its PRs).
- `CODEOWNERS` and `dependabot.yml` are deliberately **not** here — GitHub does not
  propagate them org-wide; they stay per-repo / template-driven.

Full standard: `clients/.ai/guidelines/github-standards.md` (in the workspace).
