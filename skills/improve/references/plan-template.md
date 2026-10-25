# Plan template

```markdown
# NNN: [Short imperative title]

Severity: Blocker | Major | Minor
Effort: S (under 30 min) | M (under 2 hours) | L (more)
Category: hierarchy | accessibility | consistency | responsive | motion | copy | performance

## Job
[One sentence: what the user is trying to do on this screen.]

## Problem
[What is wrong, where, and why it matters. Cite the principle.]

Evidence:
- `path/to/file.tsx:42` [what is there]

## Change
1. [step]
2. [step]

| Before | After |
| --- | --- |
| [current] | [target] |

## Do not touch
- [files, components, behaviours to leave alone]

## Verify
- [ ] [observable check, e.g. tab to the button, focus ring visible]
- [ ] Lint, types, build pass
- [ ] Checked at narrow and wide widths

## Risks
[What could break. What was not verified.]
```
