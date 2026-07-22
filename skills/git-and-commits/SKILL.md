---
name: git-and-commits
description: Guidance for creating and organizing Git commits. Use when preparing, reviewing, or making commits.
---

- Create isolated commits for each logical change.
- Commit changes and their unit tests together.
- Write descriptive commit messages that give a high-level overview of the change, why it was made, and relevant context such as alternatives considered. Do not merely describe the code itself.

- Create isolated commits; include the implementation and its tests together.

- For every non-trivial commit, write an outcome-focused subject line:
  - State the user-visible behaviour, bug, or risk addressed.
  - e.g: Prefer “Stop flaky resize tests” over “Synchronize Cypress resize assertions”.
  - Do not lead with an implementation detail unless that detail is the outcome.
  - Keep it imperative and concise.

- Include a commit body when the reason is not obvious from the subject. It must say:
  1. Why the change is needed: the observed failure, user impact, or risk.
  2. How the change addresses it, at a high level.
  3. Relevant alternatives or constraints, when they influenced the design.

- If needed, refer to the staged diff any context provided by the prompt.

- Wrap all lines to 72 characters in the commit body.