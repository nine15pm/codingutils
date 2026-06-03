---
name: task-coder
description: Use when implementing a coding task.
---

# Task Coder

## Test Writing

- OPTIONAL: Before coding, write failing TDD-like tests only for behaviors that are explicit, stable, known, and visible from a public boundary. Only when possible. Don't write tests that require guessing the implementation.

- After implementation and checking with user, write the full set of tests.

- Never mix test writing and implementation. Always stop and check in with the user before switching between them.

## Implementation

Implement the task. Before writing code, first read the relevant specs to deeply understand the intent and technical design for what we are building, and the current code progress/state.

Lazy hallucinated assumptions are never acceptable. Always verify important behavior against the authoritative source of truth. Do not purely satisfy the literal wording of a task when that leads to a suboptimal implementation; fulfill the intent using the simplest clean approach that fits the project. Do not let generic software-pattern autopilot drive the design. Do not write fake, throwaway, bridge, or guessed-at code to fill in things that should not be filled in yet.

Do not assume existing code is the right direction. Never add backward compatibility, shims, or parallel implementations by default. If the existing code no longer fits the clean approach, replace or unify it. Raise compatibility only when an external contract or user instruction requires it.

Use simple, short, concrete names in code that a new engineer can understand immediately. Never use long, abstract, convoluted, jargon-heavy names when a shorter direct name works.

Ensure that your implementation and code is tiny, clean, simple, extremely easy to consume, and not hacky. Avoid cleverness and bloat. Include comments in key places so a new person reading the code can easily follow the logic.
