# COMMON
## One-shot design + break down
We are planning out Milestone [X] in project.md. Understand the current state of the project, think through the specs for Milestone [X], and identify the key technical design decisions needed. If there are options, present them succinctly and I will decide. Then, break down the milestone into succinct and concrete tasks in an order that makes logical sense to build up the project incrementally. Do not over-index on hypothetical details that should be left to the implementing engineer. Do not write code yet.

## Tech design 1
We are planning out Milestone 9 in project.md. This is a critical piece of work to get right to support the entire future of direction of the game. First read through the specs and understand what we are trying to accomplish, understand current code progress/state, and think through the key tech design approaches. Focus on thinking through the right high-level architecture (don't get lost in the weeds) and what the simple, elegant, scalable, ideal patterns are to achieve this (like a senior game dev tech lead). If there are key decisions, highlight them along with the recommendation, explaining the why and "so what" from first principles. Do NOT anchor on existing code or try to reuse existing functions etc. that don't really fit the intended purpose, or do backward compatibility. Nothing in the current code is sacred, we can scrap, redesign, redo any part of the game we want to achieve the clean, simple, ideal end state. If there's lack of clarity or issues with the spec, flag them to me. Do not write code yet.

## Tech design 2
I'd like you to document the key architecture pieces and high level technical choices under "Tech design" in milestone9.md. Focus on the important things like what new systems we will create and why, role of existing systems (e.g. do we get rid of it, rewrite it, alter it, etc.), how functionality flows or is composed across these pieces and across server/client. Don't get bogged down in implementation details, but feel free to highlight example fields from an item schema for example, if it's helpful in illustrating the high level tech design. It should be easy to understand and a canonical reference for all eng who are implementing specific parts later. I want to stress and reiterate again - nothing in the current code is sacred, we can scrap, redesign, redo any part of the game we want to achieve the clean, simple, ideal end state. Do NOT anchor on existing code or try to reuse existing functions that don't really fit, or do backward compatibility.

## Break down into tasks
Ok, now think through the logical breakdown of tasks and sequencing of implementation. Each task should be a distinct chunk that can be assigned to an eng. Tasks should be succinct and concrete, explain what we are trying to achieve not just what we are doing. Task should not over-index on hypothetical prescriptive details that should be left to the implementing engineer. Do not write code yet.

## Plan task
We are working on Milestone 8 in project.md. The team is working on tasks in parallel. I want you to work on the 1st task. First read through the documentation and understand what we are trying to accomplish, understand current code progress/state, and think through the tech design approaches, and plan out what you need to do methodically and logically. Do not simply be constrained to what's mentioned in the task if there's a better way. If there's something in the task or an existing code implementation that is not optimal, an issue, or should be changed, flag this to me with a recommendation on ideal approach. I want to make it absolutely clear - nothing is sacred, we can scrap, redesign, redo any part of the code we want to achieve the clean, simple, ideal end state. Ensure your planned approach is absolutely clean, elegant, consistent patterns, tiny, organized, and not hacky. Do not write code yet.

## Start task
Go ahead with the first task. Go step by step in logical pieces, do not one-shot a lot of code at once. Check back after completing the task. Ensure that your implementation is clean, correct, consistent patterns, tiny, organized, and not hacky. Nothing is sacred - we can change any part of the code to achieve the clean, ideal end state.

## Debug
Root cause this logically and methodically until you have a conclusion and propose a fix. Do not write or edit any code yet.

## Test planning
Are there any essential tests we should write to validate implementation? Plan out what tests are needed for MECE coverage of all logic and edge cases. Tests should be real (not mocked/faked), written independently, and focused on guaranteeing correctness. Do not write any code yet.

## Write tests
Tests should be real, not mocked or faked. They should not know about the internal of game code we're testing (e.g. lightweight harness if needed). And they should be written independently without running them to ensure we don't hack tests to pass. Go step by step in logical pieces, do not one-shot a lot of code at once. Review your own work for global correctness and check in with me when done each set of tests.

## Review implementation 1
We're doing [X]. This will follow the spec in [X]. An eng just implemented. Review the code and flag if there are any errors or issues so far. The goal is clean elegant tech design, correct logic, simple and tiny where possible, and not hacky/bloated at all.

## Review implementation 2
Review the implementation for any issues, errors, or incorrect logic. Evaluate whether the patterns, structure, and code are in line with clean, elegant, ideal end state. Flag anything that is hacky, bloated, inconsistent, or sub-optimal. If we need to rearchitect or redo tech design to get things clean and correct, that's fine, nothing is sacred. Propose improvements. Do not write code yet.

## Rewrite/refactor 1
We're in the process of a poker system from scratch rewrite to make it clean, correct, simple, and elegant patterns, no bloat or dirty hacky stuff. Read and follow the spec in pokerrefactor.md. We are scrapping the existing PokerManager, it's bloated and incorrect, ignore it. We are going entirely from scratch, implementing based on the spec. Nothing is sacred, we can change or delete or completely do from scratch any part of the game's code, whatever is needed for the cleanest, most consistent, end state. Additionally, I don't want you to optimize for tests passing at all right now. In fact, we have deleted the old PokerManager tests. We are using pokerrefactor_execution.md as a light execution tracker. We have completed the first 4 tasks in Chunk 1. Understand what you need to do for the next task in Chunk 1, then check in with me before starting. If there's something in the task definition or ordering that is not optimal, don't be constrained by it, flag it to me. If you see an error or issue with the spec or existing code, flag this to me. Don't write any code yet.

## Rewrite/refactor 2
We need to do a major rewrite of [COMPONENT]. The current implementation is [messy/incorrect/hacky]. Understand the current status, what needs to be scrapped, redesigned, and rewritten. Plan out what needs to be done to make it clean, correct, and elegant. Nothing is sacred, we can scrap, redesign, redo any part of the codebase to achieve the clean, correct, simple, ideal end state. Do not write code yet.

## Reflect on preferences
Based on our conversation so far, are there any clear high-signal general preferences (not specific to this task or project) you can infer from our interactions that would be beneficial to call out for future coding agents? E.g. from what I've said, emphasized, asked, liked vs. seemed frustrated by, etc. If so, add succinct bullets in PREFERENCES.md to reflect these preferences in simple direct language, in a way that will get future LLM agents to behave more in line with my preferences. Don't add duplicative preferences. You can edit/update existing preferences if you have high confidence, but do not delete preferences.
