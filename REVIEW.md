# Squid Quarters review and integration

> Generated from the common section of `PREFERENCES.md` in the dotfiles at commit `801d85dafbaf11f2469e7d0875d9a003b6935b9f`.
> SHA-256 of the section text between the markers is `b3f1fec0f8955c2abfbda15b210935ac13ae9e7ecd52eb844af8cb3d99cc905c`.

<!-- BEGIN COMMON WORKING RULES -->
## Common working rules for personal projects

- **Scope.** Work on the assigned task. Respect its owner, holds, existing edits and workspace constraints. An open issue grants no assignment. An independent reviewer may inspect the change within the assignment. Get the project owner's authorization, directly or through an authorized delegate, before reassigning, delegating implementation or creating subtasks.
- **Tracking.** In personal GitHub repositories, reuse or open an issue before non-trivial work lands. Preserve issue history. Use `Closes #n` for completed work and a reference for partial work. File issues for material work left unfinished.
- **Branch and PR.** Branch from the project's actual integration branch. Use its commit convention, with Conventional Commits as the default. Integrate code, design, docs and workflow changes through a scoped PR. Never push directly to canonical or release branches. The assignment permits opening a PR and fixing findings within local ownership and push limits. Preserve required release or imported history when merging.
- **Before committing.** Use the project's required hook in your checkout and run all configured commit checks. Verify the staged snapshot when the hook checks it. Fix failures without bypassing the hook or substituting CI.
- **Independent review.** Give an independent AI or human reviewer the assignment, acceptance criteria, full diff against its base, head commit and relevant context. Scale the review to the impact. Check behavior, regressions, races, trust boundaries, failures and coverage. For design, docs and process, check usability, accessibility, voice, source accuracy, consistency, provenance and how the instructions load and work in practice.
- **Fix and verify.** Require concrete evidence and impact for material findings. Deduplicate, fix them in the same PR and explain any rejection. Repeat independent review until the final diff is clean. After fixes, rerun applicable configured checks, exercise changed flows and failures, manually test changed browser and UI flows, inspect relevant renders and verify docs against their sources. Required forge checks must pass on the reviewed head.
- **Evidence and merge.** Record the reviewed commit, reviewers, findings and dispositions, check commands and results, functional evidence and limits in the PR. Merge only within the assignment and with independent review, all required checks verified and no unresolved material findings. If the head changes, repeat affected review and checks. Distinguish local readiness, an open PR, a merge and verified delivery.
- **Release authority.** Before merging, check branch and path triggers, provider bindings and what users receive. Reviewed changes may merge to established previews or staging within the assignment. Get project-owner approval for production deployments and releases, including merges that trigger them. This includes branch updates that change what public visitors receive or users install. Record the approved target and result. Credentials, production data, real customer data, persistent access or security changes, purchases and proprietor or client design decisions require explicit authority.
- **Local rules.** Keep extra gates with the affected work. Name the surface, trigger, added evidence or permission and local source. Document a relaxation as an approved exception with the exact rule, scope, decision owner and reason. Keep existing gates during adoption.
- **Common tier.** Apply these rules to all covered work, including private or experimental work and public source. Keep applicable privacy, licensing, design approval, native interaction and testing requirements.
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
