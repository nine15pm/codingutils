---
name: tests-writer
description: Use when writing or reviewing tests.
metadata:
  short-description: Write useful, readable tests
---

# Tests Writer

- Write tests that prove real behavior and critical correctness.
- Test what the code is supposed to do, not how it is built inside. Use the smallest clear entry point for the behavior. Check results that matter to the caller or user. Do not test private details or repeat the same logic from the implementation inside the test.
- Prefer a few strong tests over many shallow ones. Prefer a few fast, strong tests of real behavior. Test logic directly.
- Avoid trivial tests, fake assertions, and tests that would still pass if the feature were broken.
- The goal is not to test every unlikely unimportant edge case, that's usually a waste of time.
- If a test fails, always stop and flag it to the user. Don't simply change implementation code to make a failing test pass.
- Keep tests small, clean, and readable. Use shared helpers for repeated setup, but avoid abstractions that make the test harder to understand.