# orbyn.dev agent instructions

This repository is the orbyn.dev site. Read [README.md](README.md) and
[CONTRIBUTING.md](CONTRIBUTING.md) before editing.

- Build and check: `node scripts/build-site.mjs --check`. The check fails on a
  broken link, inline style or script (the CSP blocks them), a GitHub link
  outside `orbyn-dev`, or wording that suggests something is out or for sale.
- Designs: the UI follows the private repository orbyn-dev/orbyn-designs, the one source of truth: `artifacts/` holds the published designs, `artifacts.json` indexes them, and `briefs/` holds the design-match brief. Read it from a current clone (`git pull` first), never from a copy in a temp folder, and never edit `artifacts/` here. Match the designs exactly, in Light, Dark and Dim, including copy and motion; take every value from the design source. A UI change cites the artifact version and frame ids it builds, or links the design pull request there. Anything not designed or not in the plan goes to the Orbyn Product UI/UX Designer before it is built; never invent it. The repository is private, so a contributor without access gets the frames they need in their issue. Public files never link the private plan or the design artifact pages (say "internal designs").
- Do not invent copy, states, dates, sign-ups or download and buy buttons.
- No product is out yet. Keep every app at Building and Teams at Planned until
  the owner says otherwise.
- Never commit `.env` or `.env.production`, and never print their values.
- `scripts/deploy.sh` deletes the old app's data. Run `--check` first, and only
  run it on a host you were asked to deploy to.
- Commit messages never carry AI attribution trailers; disclose AI use in the PR
  body only. Write your own squash message when merging (`gh pr merge --subject --body`).
