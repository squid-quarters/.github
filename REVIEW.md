# Squid Quarters review and integration

> Generated from the common section of `PREFERENCES.md` in the dotfiles at commit `7f14966fdca4fb38e522e62dec5ab66c9f4e1b82`.
> SHA-256 of the section text between the markers is `c5b676d63e3b7445e3174552fa271cbf64f4fb106ad3ee50bf516fcb6096ab45`.

<!-- BEGIN COMMON WORKING RULES -->
## Common working rules for personal projects

- **Scope.** Stay within the assignment. Respect ownership, holds, existing edits and workspace rules, including documented single-writer exceptions for tools like Unity. Open issues grant no assignment. Get project-owner approval to reassign, delegate implementation or create subtasks unless the assignment already permits it, such as an authorized orchestrator dispatch or an in-task model-routing split.
- **Tracking.** Follow documented repository tracking rules first. Otherwise, in personal GitHub repos, open or reuse an issue before non-trivial work lands. Preserve issue history. Use `Closes #n` for completed work and references for partial work. File issues for material follow-ups.
- **Branch and PR.** Branch from the project's actual integration branch. Use its commit convention, with Conventional Commits as the default. Integrate code, design, docs and workflow changes through a scoped PR. Never push directly to canonical or release branches. The assignment permits opening a PR and fixing findings within local ownership and push limits. Preserve required release or imported history when merging.
- **Before committing.** Use the project's required hook in your checkout and run all configured commit checks. Verify the staged snapshot when the hook checks it. Fix failures without bypassing the hook or substituting CI.
- **Independent review.** Independent AI or human reviewers may inspect assigned changes. Share the assignment, acceptance criteria, full diff, base, head and relevant context. Green CI, lint, self-review or a skim alone cannot satisfy independent review. Scale to impact. Check behavior, regressions, races, trust boundaries, failures and coverage. For design, docs and process, check usability, accessibility, voice, source accuracy, consistency, provenance and how instructions load and work in practice.
- **Fix and verify.** Prioritize high-confidence material findings with evidence and impact, and omit invented findings and filler nits. Deduplicate, fix them in the same PR and explain any rejection. Repeat independent review until the final diff is clean. After fixes, rerun applicable configured checks, exercise changed flows and failures, manually test changed browser and UI flows, inspect relevant renders and verify docs against their sources. Required forge checks must pass on the reviewed head.
- **Evidence and merge.** Record the reviewed commit, reviewers, findings and dispositions, check commands and results, functional evidence and limits in the PR. Merge only within the assignment and with independent review, all required checks verified and no unresolved material findings. If the head changes, repeat affected review and checks. Distinguish local readiness, an open PR, a merge and verified delivery.
- **Release authority.** Before merging, check branch and path triggers, provider bindings and what users receive. Reviewed changes may merge to established previews or staging within the assignment. Get project-owner approval for production deployments and releases, including merges that trigger them. This includes branch updates that change what public visitors receive or users install. Record the approved target and result. Credentials, production data, real customer data, persistent access or security changes, purchases and proprietor or client design decisions require explicit authority.
- **Local rules.** Keep extra gates with the affected work. Name the surface, trigger, added evidence or permission and source. For other relaxations, document the approved exception's rule, scope, owner and reason. Keep existing gates during adoption.
- **Common tier.** These rules apply only to personal projects, including private, experimental and public-source work. Keep applicable privacy, licensing, design approval, native interaction and testing requirements.
- **Public delivery tier.** For a public release of an installed tool, use the release candidate to verify the installed result through the consumer's path and verify recovery before release. For a public site, verify the intended output and rollback path before publishing and check the published output afterward. Identify the exact artifact or content, exercise relevant failures with realistic synthetic evidence and record recovery for the surface. For customer-facing transactions, also follow the project's customer-release gates, including synthetic order, payment and auth checks and staging evidence before production approval.
- **Current assignments.** The customer-release gates apply to the Flagship Games shop. The installed-tool gates apply to Hyper Chamber installers and their Homebrew casks, Svelte Lens packages and Riftbound Oracle skills. The public-site gates apply to Minor Adjustments, the shop brand guide, the Hyper Chamber site and the Riftbound Oracle site. Flagship Gains is on the common tier and keeps its privacy, emulator, CSP and build checks. Other work uses the common tier with its local rules.
<!-- END COMMON WORKING RULES -->

## Adopt this guide

Point the project's `AGENTS.md` to the reviewed revision of this guide and to
applicable local requirements. A Markdown link requires an explicit read.
Follow the project entry point and any nested instructions for the assigned
work, including when working from a control directory.

For offline or restricted jobs, provide the adopted text and revision, project
and branch or head, working directory, applicable instructions and task scope
in the brief. Reload instructions in active sessions when the adopted revision
changes. If you cannot read the adopted rules, report the missing input and
wait for it before integrating. Record the policy revision if the applicable rules could be
ambiguous. Resolve material authority conflicts with the project owner before
taking the affected action.
