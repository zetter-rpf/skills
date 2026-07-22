---
name: ruby-tests-and-rspec
description: Guidance for Ruby testing with RSpec. Use when creating, modifying, or reviewing Ruby tests.
---

# Ruby Tests and RSpec

+ Avoid deeply nested context/describe scopes. Have a describe block for each method and only use additional nesting when needed.
+ The 'act' step of the test should be in the 'it' block, not a 'before' block.
+ Instead of using stubbing, consider using dependency injection or adding a parameter to functions if simpler.
