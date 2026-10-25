# Instructions for AI agents

This is the GitHub profile repo: [README.md](README.md) is shown on <https://github.com/Alirex>. No code, no tests: the
only checks are the prek hooks.

General practices live in HQ: [evocaslab/hq `practices/`](https://github.com/evocaslab/hq/tree/main/practices)
(local clone `~/dev/hq/practices`). This file is this repo's binding version; it wins where the two differ.

## Rules

- Land directly on `main`: this is a tiny docs-only repo, so no worktree or branch is needed. Commit only when
  `prek run --all-files` passes, and push every commit right away. Read-only questions need no commit.
- Setup once per clone: `prek install` (prek: `uv tool install prek`). markdownlint needs Node.js on PATH.
- Markdown is formatted by prettier and checked by markdownlint with the default rules; `.markdownlint.yaml` turns a
  rule off only with a reason on its line. Fix the finding, don't silence it:
  [HQ lint-strictness](https://github.com/evocaslab/hq/blob/main/practices/lint-strictness.md).
- Only real, public facts in the README: public repos, links already on the GitHub profile. Never add private repos,
  company work, emails or guessed roles and numbers; ask the maintainer or leave a `TODO(maintainer)` comment.
- Badges are shields.io only (static stack badges, package versions, stars). No stat-card widgets, visitor counters or
  tracking pixels unless the maintainer asks.
- Plain Markdown that reads well in light and dark themes and on phones: lists over wide tables, no images that only
  work on one background.
- Plain, natural English: short sentences, no buzzwords.
- Commits are Conventional Commits (`docs:` for content, `chore:` for tooling), lowercase subject.
