# Project info
- project.md has a summary of the project and planned milestones/tasks

# Guidelines

## Before coding
- Think through the approach before writing any code. Understand specs and current state first.
- If there are key decisions or clarifications needed, make recommendations and check in before implementing.
- The goal is the cleanest correct end state. Don’t preserve old patterns for “compatibility.”
- If something is messy or wrong, flag it and propose the clean fix. Don’t stack more bad code on top.

## Architecture & design
- Absolutely clean, consistent, simple, elegant patterns. Nothing hacky, dirty, redundant.
- Functionality should be well organized and componentized without bloat.
- If current implementation is poorly designed, hacky, or inconsistent, flag it and suggest improvements. Don't add to bad code.
- Nothing is sacred. If rewriting or restructuring results in a cleaner end state, propose it.
- Favor simple solutions. Don't solve for hypothetical scenarios or be overly clever.
- This is not an enterprise codebase. No unnecessary boilerplate or abstraction.

## Implementation process
- Work step by step in logical chunks. Don't one-shot large changes.
- Check back after completing each chunk for review.
- Don't be constrained by task descriptions if there's a better approach.
- Consider correctness across the whole codebase, not just the immediate task.

## Code
- Tiny, clean, minimal, easy for others to understand.
- Simple folder/file structure and naming. Filenames lowercase.
- No useless wrapper functions.

## Bug fixing
- Identify the root cause before proposing changes.
- Don't rush to make changes before confirming the root cause.

## Testing
- Write minimal tests for key functionality.
- Tests should verify real behavior, not be mocked/faked just to pass.
- Write tests independently from running them to avoid hacking tests to pass.

## Communication
- Flag issues proactively. Explain the plain-English "so what" impact.
- Make concrete recommendations. Don't hedge.

## Frameworks & libraries
- Your knowledge of specific frameworks (Three.js, Colyseus, etc.) may be outdated. Reference docs or ask if unsure.
