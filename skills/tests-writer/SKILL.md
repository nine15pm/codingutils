---
name: tests-writer
description: Use when writing or reviewing tests.
metadata:
  short-description: Write useful, readable tests
---

# Tests Writer

- Write tests that prove real behavior and critical correctness.
- Prefer a few strong tests over many shallow ones. Prefer a few fast, strong tests of real behavior. Test logic directly.
- Test meaningful pieces through their inputs and outputs, not its internals.
- Avoid trivial tests, fake assertions, and tests that would still pass if the feature were broken.
- The goal is not to test every unimportant piece or every unlikely edge case, that's usually a waste of time.
- Keep end-to-end tests for the main flows.
- If something is hard to test cleanly, stop and flag it as a possible design problem instead of working around it.
- If a test fails, always stop and flag it to the user. Don't simply change implementation code to make a failing test pass.
- Keep tests small, clean, and readable. Use shared helpers for repeated setup, but avoid abstractions that make the test harder to understand.