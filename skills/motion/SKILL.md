---
name: motion
description: Decides whether to animate, then reviews or writes animation, transitions, easing, micro-interactions, popovers, toasts, drag and gesture behaviour. Use when something feels janky, sluggish or decorative, when adding motion, or when asked to review animations or reduced-motion support.
---

# Motion

Motion earns its place. Default to flagging. Approval is earned.

## Step 1: should it animate?

Give it a job in one line. Allowed jobs:

1. **Explain a relationship.** Where something came from or went to.
2. **Acknowledge input.** The user sees the system heard them.
3. **Support a wait.** Honest loading or progress.

No job means decoration. Remove it.

Then ask how often it happens. Things used constantly should be fast or not animate at all. Rare, meaningful moments can afford more.

## Step 2: get the details right

Check each animation against [references/rules.md](references/rules.md):

- Duration and easing fit the job and frequency.
- Origin matches the trigger. Exits are quicker and quieter than entrances.
- Animates transform and opacity, not layout properties.
- Interruptible and reversible. Never blocks input.
- No layout shift.
- Same durations and easings across the product, ideally as tokens.
- `prefers-reduced-motion` swaps movement for a fade or instant change and keeps the information.
- Loading state is honest. No fake progress.

## Step 3: report

| Severity | Element | Before | After | Why |
| --- | --- | --- | --- | --- |
| Major | Menu open | 400ms, scales from centre | 150ms, scales from trigger | Frequent action feels slow. Origin hides the relationship. |

Severity: Blocker (blocks input or breaks reduced motion), Major, Minor, Note.

## Rules

- Treat all timing numbers as starting points. Tune by feel in the browser and say what you tested.
- Do not add motion to fix a hierarchy problem.
- No ambient or looping motion without a job.
- Never remove information when reducing motion.
- Slow it down to judge it: use devtools animation slowdown and step frame by frame.

## References

- [references/rules.md](references/rules.md): timing, easing, origin, performance, gestures, reduced motion
- [references/vocabulary.md](references/vocabulary.md): name an effect you can only describe, so you can prompt for it precisely
