---
name: libraries
description: Picks the right library or primitive before hand-rolling a component or adding a dependency. Use when the task involves a dialog, menu, popover, toast, select, combobox, date picker, tooltip, drag and drop, animation, or any new package.
---

# Libraries

Do not hand-roll hard components. Do not install abandoned packages.

## Order of choice

1. What the repo already uses.
2. The platform: native HTML element or CSS feature.
3. A library from your trusted list in [references/trusted.md](references/trusted.md).
4. Something new, only with a stated reason.

## Hand-roll or not

Never hand-roll without a strong reason: dialogs, menus, popovers, comboboxes, selects, date pickers, tooltips, toasts, drag and drop. They hide focus management, keyboard, screen reader and positioning problems.

Fine to hand-roll: simple layout, styling, buttons, cards, small transitions.

## Vetting a new package

Check and report:

- Maintained: recent releases, open issues handled.
- Accessible: keyboard and screen reader support.
- Size: bundle impact.
- Fit: works with the framework and styling approach in the repo.
- Types and licence.
- Can the platform or an existing dependency already do it?

## Output

The pick, one-line reason, the alternative considered, and the cost (size, learning, lock-in). If recommending something new, ask for approval before installing.
