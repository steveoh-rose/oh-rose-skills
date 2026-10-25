# States checklist

Decide each state for every interactive element. Mark n/a only with a reason.

| State | Question |
| --- | --- |
| Default | Does it look interactive at rest, without hover? |
| Hover | Does it enhance the affordance without moving layout? |
| Pressed | Is there immediate acknowledgement? |
| Focus | Is the indicator visible with enough contrast? |
| Disabled | Is it clear why, and what would enable it? |
| Loading | Does it keep its size? Is it clear something is happening? |
| Error | Does it say what went wrong and how to fix it? Is input kept? |
| Success | Is completion stated? Is there a next step? |
| Empty | Is there guidance and a way forward, not a blank area? |

## Layout stability
Dimensions must not change between states. Reserve space for error text and spinners.

## Honesty
Do not show "sent" before it is sent. Labels must match what happens.

## Reversibility
If a user can lose input or trigger something irreversible, add a warning or an undo.

## Visual rules
- 4px increments on an 8px rhythm.
- One-pixel lines only for real boundaries.
- Filled surfaces for meaningful groups. No cards by default.
- Consistent control shape, radius and states.
- No gradients, badges, shadows, borders, animation or cards without a one-sentence reason that helps the user.
