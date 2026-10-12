# AGENTS.md — gear-null org conventions

Cross-repo conventions for all gear-null personal projects. Per-repo
architecture and design rules live in each repo's own `AGENTS.md` below
this preamble.

## Branching

GitHub Flow: `main` is the canonical branch. Cut feature branches from
`main`; PRs target `main`. Use `type/short-description` branch names
(`feat/…`, `fix/…`, etc.).

## Commits

Conventional Commits: `type(scope): description`.

## Pull requests

All changes land via PR — never commit directly to `main`. Keep PRs
scoped to one logical change. PRs are lightweight: a short description
of intent and key design decisions is sufficient — no template required.

## Verify before commit

Run every check the repo configures — lint, type-check, build, and
tests — and make them all pass. Do not skip checks or bypass hooks
(`--no-verify`, etc.) to push past failures; fix the underlying issue.

## Agent autonomy & pre-merge review

Read the shared [review process](https://github.com/squid-quarters/.github/blob/main/REVIEW.md)
before review or integration. It applies to code,
design, docs and workflow changes: independent substantive review (AI accepted),
material fixes, repeated review until clean, final applicable checks/tests and
PR evidence before autonomous scoped merge. Inspect publishing triggers;
deployments, credentials, production data and access/security changes require
separate task authority.

## Tracked work

Track non-trivial work in GitHub Issues before writing code; keep the
issue updated as work progresses. Trivial changes (typos, automated
bumps, single-line fixes) are exempt. Use GitHub Projects for
cross-repo visibility when needed.

## Releases

Tag GitHub Releases with semver when the change feels significant
enough to mark. No strict cadence — ship when it's meaningful.

## Agent context

`AGENTS.md` is the cross-tool source of truth for agent context.
`CLAUDE.md` is a one-line `@AGENTS.md` import. Edit `AGENTS.md` — never
`CLAUDE.md` directly. Each repo may carry its own project-specific
section below the org preamble.

## Defaults

- Stay in scope. No files created unless asked, no refactors, and no
  speculative error handling beyond the task.
