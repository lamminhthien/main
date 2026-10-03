---
name: dev-plan-validate
description: Validate an existing development plan before implementation. Use when the user invokes dev-plan-validate or asks to challenge a plan's assumptions, dependencies, and tests.
---

# Validate a development plan

Read the plan path supplied by the user, or the single relevant plan under `.agents/plans/`. If there are several plausible plans, ask which one. Inspect the referenced repository files and instructions; do not assume the plan's claims are true.

Check that the goal and acceptance criteria are observable, file references and commands exist or are explicitly to be created, steps are ordered by dependency, and the plan addresses relevant failure paths, compatibility, and tests. Challenge assumptions with code evidence. Identify missing decisions that would change implementation.

Report `PASS` or `NEEDS REVISION`. For each issue, give severity, plan section, evidence, and a concrete correction. If the plan is sound, state what was checked. Do not implement the planned change. Revise the plan only when the user asks for revision; otherwise leave the findings for `dev-plan` or the user to resolve.
