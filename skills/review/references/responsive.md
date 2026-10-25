# Responsive checklist

Widths are probes for finding where a layout breaks. Fix at the break, do not hard-code device sizes.

## Probes
320px, 375 to 430px, 768px, 1024 to 1280px, 1440 to 1920px, 2560px and above.

## At each width
- [ ] No horizontal scroll.
- [ ] Comfortable line length, not too short or too long.
- [ ] Hierarchy intact. Primary emphasis still obvious.
- [ ] Navigation reachable and visible, not behind an unmarked control.
- [ ] Primary content (images, prototypes) uses the largest reasonable space.
- [ ] Tap targets large and spaced.
- [ ] Text does not clip or overlap when it wraps.
- [ ] No fixed empty space or oversized containers.

## Input
- [ ] Touch: every action works without hover.
- [ ] Keyboard: every action works without a pointer.
- [ ] Pointer: hover enhances, never gates.

## State
- [ ] Resize does not lose focus.
- [ ] Entered content survives resize and rotation.
- [ ] Scroll position stays useful.
- [ ] Open menus and dialogs remain usable after rotation.

## Media
- [ ] Images have set dimensions or aspect ratios.
- [ ] Sizes suit the viewport.
- [ ] Video and prototypes scale without cropping key content.

## Meaning
- [ ] Same labels and meaning at every size.
- [ ] If content is deferred at small sizes, there is a clear visible way to reach it.

## Common failures
Horizontal scroll, over-long lines on wide screens, controls shrinking below target size, hidden navigation with no entry point, hover-only previews, fixed heights clipping wrapped text, images shifting layout while loading.

Output a width by result matrix (pass, fail, not tested), then findings.
