---
name: improve
description: Audits a page, section or whole codebase and returns prioritised, self-contained plans any agent can execute. Use when the user says "improve the UI", "audit this", "what should I fix first", or wants a roadmap rather than a review of one screen.
---

# Improve

`review` judges one thing. This sweeps many and ranks the work.

## Modes

- `improve` : full audit
- `improve quick` : hotspots only, top five
- `improve <category>` : one category, such as hierarchy, accessibility, consistency, responsive, motion, copy, performance
- `improve execute plans/001-<slug>.md` : carry out one plan

## Process

1. State the product's job in one sentence.
2. Map the surface: pages, routes, shared components, tokens, content.
3. Sweep each category using `review`, `motion` and `copy`.
4. Rank by impact on the user's job divided by effort. Blockers first.
5. Write one plan per finding or cluster using [references/plan-template.md](references/plan-template.md).
6. Write `plans/INDEX.md`: number, title, severity, effort, category.

## Rules

- Output plans only. Do not change code unless asked to execute.
- Every plan names exact files, the change, how to verify, and what not to touch.
- Plans must stand alone. No "as discussed".
- Group tiny related fixes. Split large ones.
- No redesigns unless asked. Preserve identity.
- No new dependencies unless the gain is clear and stated (see `libraries`).
- Point to where each problem is. Mark anything you could not verify.
