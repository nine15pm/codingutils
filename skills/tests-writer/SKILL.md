---
name: tests-writer
description: Use when writing or reviewing tests.
metadata:
  short-description: Write useful, readable tests
---

# Tests Writer

- Write tests that prove real behavior and critical correctness.
- Prefer a few fast, strong tests of real behavior over many shallow ones.
- Test meaningful pieces through its own inputs and outputs, not its internals.
- Use end-to-end tests just for the main critical flows.
- Avoid trivial tests, fake assertions, and tests that would still pass if the feature were broken.
- The goal is not to test every unimportant piece or every unlikely edge case, that's usually a waste of time.
- If something is hard to test cleanly, stop and flag it as a possible design problem instead of working around it.
- If a test fails, always stop and confirm the root cause. Then flag it to the user. Don't just change code or the test to make it pass.
- Keep tests small, clean, and readable. Use shared helpers for repeated setup, but avoid abstractions that make the test harder to understand.
- A flaky test is a bug. Fix it or delete it.