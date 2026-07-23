---
name: git-and-commits
description: Guidance for creating and organizing Git commits. Use when preparing, reviewing, or making commits.
---

- Create isolated commits for each logical change.
- Commit changes and their unit tests together.
- Write descriptive commit messages that give a high-level overview of the change.

- For every commit write an outcome-focused subject line:
  - State the user-visible behaviour, bug, or risk addressed.
  - e.g: Prefer “Stop flaky resize tests” over “Synchronize Cypress resize assertions”.
  - Do not lead with an implementation detail unless that detail is the outcome.
  - Keep it imperative, concise and under 72 characters.

- For every commit include a commit body. It must say:
  1. Why the change is needed: the observed failure, user impact, or risk. (Can start with 'Previously..' )
  2. How the change addresses it, at a high level. (Can start with 'This change..' )
  3. (optional) Relevant alternatives or constraints, when they influenced the design (Can start with 'Alternatively..').
  4. (optional) Any relevant references/links such as documentation.

- For simple changes and new features the commit body might just be one short sentence. For more complex changes it may be a few paragraphs.
- If needed, refer to the staged diff any context provided by the prompt.
- Wrap all lines to 72 characters in the commit body.