# Contributing to the shared CodeRabbit settings

Thank you for helping. This repository holds one file, `.coderabbit.yaml`, which
CodeRabbit uses for every SureForgeTech public repository that has no file of
its own. The general guide for all SureForgeTech repositories is the
[organization contributing guide](https://github.com/SureForgeTech/.github/blob/main/CONTRIBUTING.md);
this page adds what is specific here.

## How to contribute

Issues and pull requests are welcome.

- **Sign off every commit** with `git commit -s`. This adds a `Signed-off-by:`
  line certifying the [Developer Certificate of Origin](https://developercertificate.org/).
  A check confirms the sign-off on pull requests from outside contributors.
  If it fails, amend the commits with `git commit -s --amend` (or
  `git rebase --signoff` for several) and force-push the branch with
  `--force-with-lease`.
- **Your contribution comes under the licence in the `LICENSE` file** (Apache
  License 2.0).
- **Every pull request gets review** and must pass the required checks before a
  maintainer merges it.

## What to keep in mind

- A change to `.coderabbit.yaml` affects how CodeRabbit reviews **every**
  SureForgeTech public repository that has no file of its own. Explain in the
  pull request what changes for reviewers and why.
- A repository's own `.coderabbit.yaml` always wins over this one.
- CodeRabbit reviews are advice only and never required. If no review appears
  on a pull request, comment `@coderabbitai review`.
- Keep private information out of this repository, and never include secrets
  or tokens.
- Security problems: do not describe them in a public issue. See the
  [organization security policy](https://github.com/SureForgeTech/.github/blob/main/SECURITY.md).
