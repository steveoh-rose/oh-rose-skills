# Motion vocabulary

Use the right word when asking for an effect. Edit and extend this list as you learn terms.

| Term | What it looks like | Good for |
| --- | --- | --- |
| Fade | Opacity changes, nothing moves | Subtle state change, reduced-motion fallback |
| Crossfade | One element fades out as another fades in, in place | Swapping content of the same shape |
| Slide | Element moves along one axis into or out of view | Drawers, sheets, toasts |
| Scale in (pop) | Grows from slightly smaller to full size, usually with fade | Popovers, menus, dialogs |
| Origin-aware scale | Scales from the trigger point, not the centre | Popovers and dropdowns |
| Stagger | Items enter one after another with small delays | Lists, grids, grouped content |
| Spring | Moves with physical overshoot and settle | Drag release, playful moments |
| Rubber-banding | Resists and stretches past a boundary, then snaps back | Scroll edges, drag limits |
| Momentum | Keeps moving after release, then decelerates | Scrolling, flicking, drag release |
| Snap | Settles to the nearest defined position | Carousels, sheets, sliders |
| Shared element transition (morph) | An element moves and resizes between two views | List to detail |
| Skeleton | Placeholder shapes matching final layout | Loading content |
| Shimmer | Light sweep across a skeleton | Signalling loading, use sparingly |
| Parallax | Layers move at different rates on scroll | Depth, rarely needed |
| Marquee | Continuous horizontal scroll | Logos, tickers, usually decoration |
| Reveal on scroll | Element animates in as it enters the viewport | Long pages, use with restraint |
| Collapse and expand | Height animates open or closed | Disclosure, accordions |
| Press feedback | Slight scale or shade change on press | Buttons, cards |
| Pulse | Repeating scale or opacity change | Attention, notifications, use rarely |
| Number tween | Value counts up or down | Counters, changing totals |

## Describing an effect for a prompt

Give: trigger, what moves, from where to where, how long it feels, what the easing feels like, and what stays still. Example: "On click, the menu scales in from the button (origin at the button), short duration, ease out. Fade only under reduced motion."
