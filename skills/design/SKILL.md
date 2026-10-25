---
name: design
description: Designs or reshapes screens, sections and components. Use when the user asks to design, mock up, lay out, restyle or redesign UI, or asks how something should look or behave. For critiquing finished work use review.
---

# Design

Rule: **good design solves the job to be done.**

## Process

1. State the job in one sentence: what is the user trying to do, and what is the shortest honest path?
2. Inspect what exists. Reuse tokens, components and patterns before inventing.
3. Pick one primary emphasis. Everything else supports it.
4. Build structure with content, type and space. Add boxes, lines, colour and motion last, each with a reason.
5. Cover states: default, hover, pressed, focus, disabled, loading, error, success, empty.
6. Check narrow and wide.
7. Run `review`.

## Principles

- One hierarchy. One primary emphasis per screen.
- Make the path legible: where to start, where a link goes, when an action is done.
- Be honest. Labels and status match what is happening.
- Plain language. Labels describe outcomes.
- Interaction is visible at rest. Hover enhances, never reveals.
- Colour carries meaning only. No colour-only status.
- Space before boxes and lines.
- Stable layout. States do not shift neighbours.
- Immediate feedback. Reversible actions. Guard destructive ones.
- No dead ends. Always a next step or way back.
- Animate to explain, acknowledge or support a wait.
- No all-caps. Use size and weight.
- Primary content gets the most room. Size to content.
- Stay consistent. Use a 4px scale on an 8px rhythm.

## Rules

- Preserve existing identity unless a redesign is asked for.
- If the repo has tokens or components, use them. Do not invent a parallel system.
- Every gradient, shadow, badge, border, card or animation needs a one-sentence reason that helps the user.

## Output

The job, the structure, key decisions with a reason each, states covered, open questions. Short.

## References

- [references/principles.md](references/principles.md): all 25 design principles plus the 8 human-centred principles
- [references/states.md](references/states.md): states checklist and visual rules

For animation, use `motion`. To pick a component library, use `libraries`.
