# SureForgeTech CodeRabbit settings

This repository holds the shared [CodeRabbit](https://coderabbit.ai) configuration for the SureForgeTech public repositories. CodeRabbit reads `.coderabbit.yaml` here for any repository in the org that has no `.coderabbit.yaml` of its own. A repository's own file always wins.

## What it does
- Reviews pull requests into `main` only; skips drafts, Dependabot and other bot pull requests, and titles marked WIP.
- Reviews only new changes on later pushes, and pauses auto-review after 3 reviewed pushes.
- Skips lockfiles, generated, vendored, minified and build files, changelogs and licence notices.
- Asks for comments on bugs, security, missing tests and accessibility, with few style remarks.
- Uses the "chill" profile: no poem, no sequence diagrams.

## Free-plan limits and what happens when they are hit
CodeRabbit's open-source plan allows a small number of pull request reviews per developer per hour (documented as 1 to 10, varying with repository stars, and scoped per repository). Public repositories with fewer than 10 stars are not reviewed automatically; comment `@coderabbitai review` on the pull request to start one.

When the limit is reached, CodeRabbit comments that it is rate limited and posts a passing "Review rate limited" check. No review runs and nothing is queued. Comment `@coderabbitai review` later to retry.

Contributors: if no CodeRabbit review appears on your pull request, comment `@coderabbitai review`.

## A CodeRabbit review is never required
CodeRabbit is advice only. It is not a required check in any ruleset. Merging depends on our normal independent review of the exact head and green required checks. A rate-limited or skipped CodeRabbit review never blocks a merge.

## Privacy
Install the CodeRabbit GitHub App on selected public repositories only, never on "All repositories". Private code must not be sent to CodeRabbit.

Licensed under the [Apache License 2.0](LICENSE).
