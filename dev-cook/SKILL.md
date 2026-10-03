---
name: dev-cook
description: Implement an existing development plan and verify the requested behavior. Use when the user invokes dev-cook with a plan or asks to execute a development plan.
---

# Implement a development plan

Read the specified plan, or the single relevant plan under `.agents/plans/`, and the repository instructions. If validation findings exist, resolve blocking findings before editing. Confirm the plan still matches the code; update the plan only for a necessary implementation correction and explain the change.

Implement every in-scope acceptance criterion in dependency order. Preserve unrelated work in the shared tree. Run the plan's relevant checks and observe the behavior through its real surface where feasible. Fix failures caused by the change. If a check cannot run, record the exact reason and what remains unverified.

Report changed files, acceptance criteria met, commands and results, and any remaining blocker. Do not commit, push, or open a PR in this workflow.
