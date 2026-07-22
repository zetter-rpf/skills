---
name: js-tests-and-jest
description: Guidance for JavaScript and TypeScript testing with Jest. Use when creating, modifying, or reviewing JavaScript or TypeScript tests.
---

# JavaScript Tests and Jest

+ Avoid deeply nested context/describe scopes. Have a describe block for each function and only use additional nesting when needed.
+ The 'act' step of the test should be in the 'it' block, not a 'before' block. Helper functions can be used to reduce duplication if necessary.
+ Instead of using mocking, consider using dependency injection or adding a parameter to functions if simpler.
