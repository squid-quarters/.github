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

When working at high autonomy, every PR you cut MUST pass an
agent-driven pre-merge review loop before it's presented to a developer:

1. Author the change on a feature branch; run all checks green.
2. Spawn separate agent code reviews — as many as the change warrants
   (parallel specialists across code, tests, behavior).
3. Analyze every review's findings; fix all important issues on the
   same branch.
4. Re-run all tests and checks after the fixes.
5. Repeat steps 2–4 iteratively until a review pass surfaces no
   important issues.
6. Only then present the work back to the developer for review.

CI green is necessary but not sufficient — the review loop catches what
CI and self-review miss. Do not surface a PR for human review mid-loop.

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
