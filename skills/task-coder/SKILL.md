---
name: task-coder
description: Use only when the user explicitly invokes this skill. Do not proactively use.
---

# Task Coder
## General notes
- You are responsible for the end state of the codebase, not just completing this task. Writing working code is not sufficient. It is just as critical to have the codebase be extremely simple, clean, consistent, with good implementation patterns and very readable code. Like it's made by Anthropic or OpenAI.

## Tests
- (OPTIONAL) When it's productive, write failing TDD-like tests before coding, for behaviors that are explicit, stable, known, and visible from a public boundary. Don't write tests that require guessing the implementation, this just wastes time.
- After implementation, write the full set of tests. Don't mix test writing and implementation. Keep these independent to avoid hacking implementation to pass tests.

## Implementation
- Before writing code, first deeply understand the intent, technical design, and current state. Both the immediate task and the broader context.
- Understand and fulfill the intent. Don't blindly overfit to literal wording or assumptions that don't make sense if they lead to poor implementation.
- Don't just blindly assume existing code is the right direction. Never add backward compatibility, shims, or parallel implementations. If the existing code doesn't fit the clean approach, replace or unify it. Raise compatibility only when truly needed (e.g. external contract).
- Ensure code is very simple, clean, organized, and extremely readable. Prefer DRY, YAGNI implementation. Use consistent and cohesive patterns across the codebase.
- Avoid overengineering, overcomplication, and bloat, favor simple solutions when possible.
- Avoid overdefensive code guarding for completely impractical unimportant things.
- Avoid convoluted, hacky, inconsistent patterns (random hardcoding, useless wrapper functions, etc.).
- Annotate code with succinct comments in key places so a new person reading the code can easily follow the logic.
- Use simple, short, conventional names in code that are obvious to understand. Naming patterns need to be consistent across the codebase, follow a rough system. Don't invent unnecessary new terms or abstract, convoluted, jargon-heavy names.
- Never make lazy assumptions about things that are easily verifiable, like 3rd party libraries or API behavior. Always check the authoritative source of truth or ask the user to help you check if needed.
