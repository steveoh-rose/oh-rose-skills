---
name: review
description: Strict review of a design or implementation, including accessibility, responsive behaviour and motion. Use when the user asks to review, crit, audit, check accessibility, check mobile, or "is this good", and before calling UI work done. Default to flagging.
---

# Review

Review the real thing, not the intent. Default to flagging. Approval is earned.

## Crit

1. **Cold read.** Can you state the screen's job in one sentence?
2. **Hierarchy.** One clear primary emphasis?
3. **Deletion.** What can go without losing clarity?
4. **Path.** Is the next step obvious? Is there a way back?
5. **Consistency.** Spacing, type, controls and states match the system?
6. **Truth.** Every claim, label and status accurate?
7. **Function.** Which interactions and checks were actually run?

## Accessibility

- Semantic HTML, logical headings.
- Full keyboard use, visible focus, sensible order. Never remove focus indicators.
- Names for icon-only controls. Useful alt text, or empty alt if decorative.
- Contrast: 4.5:1 text, 3:1 large text and UI boundaries.
- Not colour alone. Labelled fields, plain-language errors, input kept after errors.
- Dialogs and menus manage focus.
- `prefers-reduced-motion` respected.

## Responsive

- Probe about 320, 768, 1280 and 1920px or wider.
- No horizontal scroll. Reflow, do not just stretch.
- Same meaning and labels at every size.
- Touch targets at least 44px. No hover-only discovery.
- State survives resize and rotation.

## Motion

- Each animation does one of: explain a relationship, acknowledge input, support a wait. Otherwise flag it.
- Responsive to input, interruptible, no layout shift.
- Prefer transform and opacity.

## Output

Verdict in one line: ship, ship after fixes, or rethink. Then a table:

| Severity | Where | Before | After | Why |
| --- | --- | --- | --- | --- |

Severity: **Blocker** (breaks the job, accessibility or truth), **Major** (clear principle violation), **Minor**, **Note**.

Finish with what was not checked.

## Rules

- Never say "looks good" without naming what you verified.
- Never claim something works untested. Write "not tested".
- Separate taste from principle. Taste is a Note.
- Five real findings beat fifteen vague ones.
- Fix, re-run once, stop.

## References

- [references/crit.md](references/crit.md): prompts for each crit point
- [references/accessibility.md](references/accessibility.md): full accessibility checklist
- [references/responsive.md](references/responsive.md): full responsive checklist

For a deep animation review, use `motion`. To sweep a whole codebase and rank fixes, use `improve`.
