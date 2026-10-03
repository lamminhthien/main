---
name: dev-plan
description: Write an implementation plan for a requested code change before implementation. Use when the user invokes dev-plan or asks for a concrete development plan.
---

# Development plan

Inspect the repository, its instructions, and the relevant code and tests. Resolve routine design choices from evidence. Ask only about decisions that materially change the result.

Write one plan at `.agents/plans/<short-slug>.md` in the target repository. Create the directory if needed. Include:

- Goal and observable acceptance criteria.
- Current behavior and the code locations that matter.
- Ordered implementation steps with specific files or modules, dependencies, and migration or compatibility work where applicable.
- Verification commands and manual scenarios that would expose a wrong result.
- Known risks, assumptions, and decisions still requiring the user.

Keep the plan scoped to the request. Do not implement the change in this workflow. Return the plan path and summarize any unresolved decision.
