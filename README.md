# Skills

Nine skills. Each `SKILL.md` is short. Longer material lives in `references/`, one level deep, and is only read when needed.

```
skills/
  brief/       references: template, task-vs-project, opportunity-tree
  design/      references: principles, states
  review/      references: crit, accessibility, responsive
  motion/      references: rules, vocabulary
  improve/     references: plan-template
  copy/        references: banned-phrases, case-study-template
  research/    references: signals
  build/       references: pre-flight
  libraries/   references: trusted
```

| Skill | Use for |
| --- | --- |
| `brief` | Scoping ambiguous or 0-to-1 work |
| `design` | Designing screens and components |
| `review` | Critique, accessibility, responsive checks |
| `motion` | Deciding on, reviewing and naming animation |
| `improve` | Auditing a codebase into ranked plans |
| `copy` | Writing interface text and case studies |
| `research` | Choosing a UX research method |
| `build` | Implementing UI code |
| `libraries` | Picking a library before hand-rolling |

## Install

Copy the folders into `.claude/skills/` (or `.agents/skills/`).

## Adjust

- Edit each `description` to change when a skill fires. Add the phrases you actually type.
- Fill in `libraries/references/trusted.md` with the packages you trust.
- Extend `motion/references/vocabulary.md` as you learn terms.
- Add a skill by copying any folder.

Priority when guidance conflicts: the explicit request, then the existing implementation, then these skills.
