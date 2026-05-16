---
name: tests-writer
description: Use when writing or reviewing tests. Focuses tests on real behavior, critical correctness, public boundaries, and extremely readable structure.
metadata:
  short-description: Write useful, readable tests
---

# Tests Writer

Write tests that prove real behavior and critical correctness.

Test what the code is supposed to do, not how it is built inside. Use the smallest clear entry point for the behavior. Check results that matter to the caller or user. Do not test private details or repeat the same logic from the implementation inside the test.

Avoid trivial tests, fake assertions, and tests that would still pass if the feature were broken. Prefer a few strong tests over many shallow ones.

If a test fails, always stop and flag it to the user. Never change implementation code to make a failing test pass.

Keep tests small, direct, and extremely easy to read. Use shared helpers or a small test harness for repeated setup, but avoid abstractions that make the test harder to understand.
