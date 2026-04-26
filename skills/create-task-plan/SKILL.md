---
name: create-task-plan
description: Create a detailed execution plan for a specific coding task before implementation. Use when the user asks to create a task plan, plan implementation, write a taskplan, or think through a coding task before making changes. Do not use for high level milestone or project planning.
---

# Create Task Plan

You are in planning mode for a task.

Hard rules:
- Do not edit source files.
- Do not modify files outside `docs/taskplans/`.
- Do not run commands that modify state, except creating or updating the task plan file.
- Read/search the repo as needed to understand the codebase, docs, current progress, and task intent.
- Ask at most 2-3 blocking questions if the plan would otherwise be wrong.
- Do not ask trivial questions; choose sensible defaults.
- Do not include unanswered questions inside the final plan unless they are truly blocking.

Planning principles:
- Start by reading the relevant docs and code to understand the intended product behavior, architecture, and current implementation state.
- Think through the technical design methodically before proposing implementation steps.
- Do not blindly follow existing docs, task wording, or code if there is a better approach.
- If the task, docs, or existing implementation seem suboptimal, fragile, overbuilt, inconsistent, or wrong, flag it and recommend the cleaner expert approach.
- Prefer simple, DRY, YAGNI implementation.
- Use test/verification-driven development:
  - Write tests before implementation whenever practical.
  - Otherwise define clear verification steps that prove the task is done.
  - Verification should reflect the minimum real gate for completion, not superficial checks.

When ready, create or update a markdown plan file in:

`docs/taskplans/`

Use this filename format when the milestone number can be inferred:

`m<milestone-number>-<short-task-name>-plan.md`

Example:

`docs/taskplans/m1-auth-routing-plan.md`

If the milestone number cannot be inferred from the task, docs, branch, or existing task plans, omit the milestone prefix:

`docs/taskplans/<short-task-name>-plan.md`

The plan must be concise, specific, and actionable.

Use this format:

```markdown
# Plan: <short title>

## Goal
One or two sentences describing the intended outcome.

## Context
Brief summary of relevant docs, current code state, and task intent.

## Scope
What will change, and what will not change.

## Tech design
Key technical decisions, architecture notes, data flow, interfaces, edge cases, or tradeoffs.

If the requested approach is not ideal, explain the better approach here.

## Relevant files
- `path/to/file.ts` - why it matters
- `path/to/test.ts` - expected test coverage

## Implementation steps
1. Concrete step.
2. Concrete step.
3. Concrete step.

Each step should be independently reviewable.

## Tests / verification
- Tests to add or update, ideally before implementation.
- Exact commands to run.
- Manual app verification steps if needed.

## Risks
- Real risks only.
- Include likely failure modes or areas needing extra care.

## Open questions
Only include unresolved questions that are truly blocking.
```

Do not over-engineer. Keep the plan proportional to the task.
Wait for explicit user approval before implementation.
