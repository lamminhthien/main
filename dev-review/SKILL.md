---
name: dev-review
description: Review implemented changes against a development plan and report actionable findings. Use when the user invokes dev-review or asks for a plan-based code review.
---

# Review a planned change

Read the specified plan, or the single relevant plan under `.agents/plans/`, and inspect the actual diff against its intended base. Check each acceptance criterion and relevant edge cases, tests, security, compatibility, and unintended changes. Run targeted checks when they can establish or disprove a concern. Do not edit code during this workflow.

Lead with actionable findings ordered by severity. For each finding, cite the file and line, explain the failure scenario, and propose a bounded fix. Distinguish observed defects from unverified risks. If there are no findings, say so and list the checks performed and any verification gap. End with whether the change is ready for `dev-ship`.
