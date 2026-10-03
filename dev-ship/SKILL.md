---
name: dev-ship
description: Run final checks, commit and push a completed change, and open a pull request without merging. Use only when the user invokes dev-ship or explicitly asks to ship a change.
---

# Ship a completed change

Treat an explicit `dev-ship` invocation for the current repository as authorization to commit the in-scope change, push its branch, and open a pull request. Do not merge or deploy.

Read the relevant plan and review findings if present. Confirm the current repository, branch, base branch, diff, and GitHub authentication. Stop with a clear reason if the intended repository or base is unclear, the branch is protected or is the base branch, review has unresolved blocking findings, unrelated changes cannot be excluded, or authentication is unavailable.

Run the plan's final checks. Stop on a failed check; report the command and failure. Stage only files belonging to the change, inspect the staged diff, then create a descriptive commit. Push the branch and open a PR against the intended base with a concise summary and check results. If an open PR already exists for the branch, report its URL instead of creating a duplicate. Never force push. Report the commit and PR URL, or the precise step and reason that stopped shipping.
