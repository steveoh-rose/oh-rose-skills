# Motion rules

Starting points, not laws. Tune by feel and keep what users can perceive.

## Purpose and frequency
- Explain a relationship, acknowledge input, or support a wait.
- If removing it loses nothing, remove it.
- Frequent, repeated interactions: faster or no animation.
- Rare, meaningful moments can be slower and richer.

## Timing (starting ranges)
- Press and toggle feedback: perceptibly immediate.
- Small state changes (hover, focus, tooltips): short.
- Menus, popovers, panels entering or leaving: short to medium.
- Page or large layout transitions: medium. Avoid long.
- Nothing the user waits through should feel slow.

## Easing
- Entering or responding: ease out (fast start, soft landing).
- Moving between positions on screen: ease in-out.
- Leaving: ease in or a quick ease out.
- Linear only for continuous progress.
- Avoid bounce and overshoot unless it carries meaning.

## Origin and direction
- Animate from where it came from. A popover scales from its trigger, not its centre.
- Transform origin should match the anchor.
- Exits are quicker and quieter than entrances.

## Performance
- Prefer transform and opacity.
- Avoid animating width, height, top, left, margin or large box-shadows.
- Do not leave `will-change` on everything.
- Check for dropped frames while scrolling and during route changes.

## Interruption and input
- Keep input live during animation.
- Reverse cleanly if the user changes their mind mid-way.
- Prefer transitions over keyframes for things that can be interrupted, because a transition can retarget from its current value.

## Stagger
- Short delays between items to show grouping. Keep the total short.
- Skip stagger on frequent interactions.

## Gestures and physical motion
- Drag follows the pointer directly, with no easing lag.
- Decide dismiss or commit using velocity as well as distance.
- Past a boundary, add resistance (rubber-banding) rather than a hard stop.
- On release, continue from the current velocity (momentum) and settle with a spring or decay.
- Touch alternatives must exist for anything that depends on a gesture.

## Stability
- No layout shift during or after a state change.
- Reserve space for loaders, errors and success states.

## Reduced motion
- Respect `prefers-reduced-motion`.
- Replace movement (slide, scale, parallax) with a fade or instant change.
- Keep the information the motion carried. A panel must still clearly open.

## Loading
- Show progress only if it is real.
- Prefer placeholders that match the final layout.
- Skip spinners for waits under about a second.

## Debugging
- Slow animations in devtools to judge easing and origin.
- Step frame by frame to catch jumps and flicker.
- Test on a slower device or with CPU throttling.
- Play it at real speed before approving. Slow-motion fixes can feel wrong at full speed.
