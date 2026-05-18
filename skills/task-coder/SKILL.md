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

Ensure that your implementation and code is tiny, clean, simple, extremely easy to consume, and not hacky. Avoid cleverness and bloat. Include comments in key places so a new person reading the code can easily follow the logic.
