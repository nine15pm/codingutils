---
name: docs-writer-astra
description: Use only when the user explicitly invokes this skill. Do not proactively use.
---

# Docs Writer

Write docs that are clean, organized, and extremely easy to understand.

## General guidelines

- Be direct, clear, succinct, and logically coherent.

- Avoid bloat. No vague filler, jargon, or empty statements that sound relevant but say little.

- Avoid overly hard prescriptive language or narrow rules, unless truly needed to spec out. It's preferable to convey the approach, intent, rationale, etc. Otherwise, agents will blindly overfit to words/rules while completely missing the intent.

- Use simple and organized doc structure. Avoid complex formatting and random one-off points.

- Avoid implicit references to irrelevant and out-of-context intermediate discussions. E.g. in a discussion you propose X+Y, user says "X is irrelevant", you remove X, then in a doc you say "Solution is Y (do not include X)". "Do not include X" is completely meaningless and actively confusing.

## Writing style
- Use the most direct and simplest possible plain English words and sentence structure. But obviously use established technical terms when they are most precise and keep technical terms, product terms, etc. exact. Think ASD-STE100 Simplified Technical English.

- Prefer the active voice.

- Prefer simple tenses: present, past, and future.

- Use the same words for the same idea or thing each time.

- No jargon. Don't invent jargon or shorthand.

- Avoid mannered prose.

- Avoid AI slop, e.g. emdashes.

- No puffery or empty emphasis. Drop words that add emphasis but no information.
