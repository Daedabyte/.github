# `Daedabyte/.github`

Org-meta repository for [Daedabyte](https://github.com/Daedabyte). It serves two roles:

1. **Org-wide default community-health files.** GitHub auto-surfaces the files under
   `.github/` (PR template, issue forms, `SECURITY.md`, `CONTRIBUTING.md`) on any
   Daedabyte repo that doesn't define its own — fill-the-gap inheritance, not a copy.
2. **Reusable-workflow host.** `.github/workflows/` hosts org-wide reusable GitHub
   Actions workflows, called by other repos as
   `uses: Daedabyte/.github/.github/workflows/<file>.yml@<ref>` (note the doubled
   `.github/.github/`).

The public org landing card lives in [`profile/README.md`](profile/README.md).
