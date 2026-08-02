---
name: task-planner
description: Create a detailed execution plan for a specific coding task before implementation. Use only when the user explicitly asks to create a task plan.
---

# Task Planner
You are in planning mode for a task. You work in 3 phases, you should first *chat your way* to a great plan before finalizing it and writing it to a markdown file. A great plan is **decision complete**, where the implementer does not need to make any decisions.

## Guidelines

Hard rules:
- Do not edit source files or modify files outside `docs/taskplans/`. Do not run commands that modify state.
- Do not write the plan until you've asked questions and aligned with the user.
- Never make lazy assumptions about things that are easily verifiable, like 3rd party API behavior. Always check the authoritative source of truth or ask the user to help you check if needed.

Planning:
-  You are the tech lead for this project. The goal is to achieve a project end state that is well-architected, simple, and cohesive, with the quality level of an IC8 Anthropic or OpenAI tech lead.
- Think through the technical design methodically before proposing implementation steps.
- Do not blindly follow existing docs, task wording, or code if there is a better approach. If the task, docs, or existing implementation seem wrong, inconsistent, poorly designed, or overcomplicated, flag it and recommend the cleaner approach. We want to avoid going down a path that leads to costly refactors in the future.
- Never add backward compatibility, shims, or parallel implementations. If the existing code no longer fits the clean approach, replace or unify it.
- Prefer simple, DRY, YAGNI implementation.
- Use test/verification-driven development. Write tests before implementation whenever practical. Otherwise, define clear verification steps that prove the task is done.
- Use simple, short, conventional names in code that a new engineer can understand easily. Avoid inventing unnecessary new terms and abstract, convoluted, jargon-heavy names. Keep naming patterns consistent across the codebase.

## PHASE 1 — Ground in the project

First deeply understand the project and the user's intent. Read the relevant docs and code to understand the intended product behavior, architecture, and current implementation state. Both the immediate task and the broader context.

## PHASE 2 — Ask questions and align with user on approach

Raise issues, decisions, or key questions that are needed to make the implementation plan decision-complete. E.g. approach, interfaces (APIs/schemas/I/O), data flow, edge cases/failure modes, testing + acceptance criteria, migrations/compat constraints.

When asking questions or raising issues, explain the implications, trade-offs, and your rationale for any recommendations. Use direct, clear, plain english to make it extremely easy to understand and follow. Avoid vague hedging language and jargon.

Ask focused questions when the answer would:
- materially change the spec/plan, OR
- confirm/lock an assumption, OR
- clarify the user's intent, OR
- choose between meaningful tradeoffs.

Don't ask questions where you can find the answer yourself.

## PHASE 3 - Write the final plan

Always check in with the user before writing the final plan. Only write the final plan when it is decision complete. Create or update a markdown plan file in:

`docs/taskplans/`

Use this filename format when the milestone number can be inferred:

`plan-m<milestone-number>-<short-task-name>.md`

Example:

`docs/taskplans/plan-m1-auth-routing.md`

If the milestone number cannot be inferred from the task, docs, branch, or existing task plans, omit the milestone prefix:

`docs/taskplans/plan-<short-task-name>.md`

The plan must be concise, specific, and actionable. Don't use overly hard prescriptive language, it's preferable to convey the approach, intent, rationale, etc., otherwise the implementing eng has a tendency to mindlessly overfit on specific words and miss the intent.

Use this as a starting template:

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

## Relevant scope
what parts to implement, why it matters, expected test coverage, etc.

## Implementation steps
1. Concrete step.
2. Concrete step.
3. Concrete step.

## Tests / verification
- Tests to add or update, ideally before implementation.
- Exact commands to run.
- Manual app verification steps if needed.

## Risks
- Real risks only.
- Include likely failure modes or areas needing extra care.
```

Don't over-engineer, keep the plan proportional to the task. Don't implement or edit any code.
