# Accessibility checklist

Mark each: pass, fail, not tested, n/a. Blockers here block shipping.

## Structure
- [ ] One `h1`. Headings nest without skipping.
- [ ] Landmarks: `header`, `nav`, `main`, `footer`.
- [ ] Buttons are buttons, links are links, lists are lists.
- [ ] Link text makes sense out of context.
- [ ] Descriptive page `title`, `lang` set.

## Keyboard
- [ ] Everything reachable with Tab, in reading order.
- [ ] Visible focus on every focusable element.
- [ ] No keyboard traps.
- [ ] Skip link on pages with long navigation.
- [ ] Custom controls support expected keys (Enter, Space, Escape, arrows).

## Names and labels
- [ ] Icon-only controls have accessible names.
- [ ] Fields have visible labels tied to inputs.
- [ ] Required fields marked in text, not colour alone.
- [ ] Related inputs grouped with `fieldset` and `legend`.

## Images and media
- [ ] Informative images have useful alt. Decorative images have empty alt.
- [ ] Captions where speech carries meaning.
- [ ] Autoplaying motion can be paused or is absent.

## Colour and contrast
- [ ] Text 4.5:1. Large text 3:1.
- [ ] Meaningful UI boundaries and icons 3:1.
- [ ] Status shown by more than colour.
- [ ] Both themes checked if both exist.

## Forms and errors
- [ ] Errors say what went wrong and how to fix it.
- [ ] Errors tied to the field and announced.
- [ ] Input preserved after an error.
- [ ] Success stated clearly.

## Dialogs and menus
- [ ] Focus moves in on open, stays contained, returns on close.
- [ ] Escape closes.

## Motion and size
- [ ] `prefers-reduced-motion` handled.
- [ ] Nothing flashes more than three times a second.
- [ ] Targets at least 44px where practical.
- [ ] Usable at 200 percent zoom.

## Rules
- Do not claim compliance. Say what was checked.
- Say if no automated tool ran.
- Fix with semantic HTML before ARIA.
