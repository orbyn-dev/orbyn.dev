# Contributing to orbyn.dev

Engineering work uses the [Orbyn Engineering workspace](https://github.com/orbyn-dev/orbyn-fullstack-skills),
with this repository cloned at `repo/Orbyn` and task worktrees at
`repo/orbyn-wt/<purpose>/`. Coding agents start with [AGENTS.md](AGENTS.md).

## Changes

1. Branch from `main` with a purpose name: `feat/`, `fix/`, `docs/` or `chore/`.
2. Run `node scripts/build-site.mjs --check`. For deploy changes, also run
   `bash -n scripts/deploy.sh` and `./scripts/deploy.sh --check` on a test host.
3. For visible changes, compare the page with the internal designs at 1160, 820
   and 390 px, in light and dark, and attach the screenshots.
4. Open a pull request and fill in every section of the template, including
   AI usage.
5. Commit messages carry no AI attribution trailers ("Co-Authored-By" naming an
   AI tool, "Generated with", a robot-emoji line). Disclose AI use in the pull
   request's AI usage section only. CI fails a pull request whose commits have
   one; when you merge, write your own squash message.
