# Crit prompts

Ask these against the real implementation.

## Cold read
- Cover everything but the first screen. What is this for?
- Would a first-time user say the same sentence? If not, hierarchy or copy is wrong.

## Hierarchy
- Where does the eye land first? Is it the intended element?
- Do two things compete at the same weight?
- Is hierarchy made with size and weight, not caps, colour or boxes?

## Deletion
- Remove each element in turn. What gets worse? If nothing, delete it.
- Look hardest at badges, dividers, cards, gradients, shadows, decorative motion, repeated labels.

## Path
- Where does the user start? Where next?
- Does each link say where it leads?
- Is there a way back from every state? Does the end of a flow offer a next step?

## Consistency
- Same spacing scale, radius, type sizes, control heights?
- Same interaction language as elsewhere?
- Any raw values where a token exists?

## Truth
- Does every claim match what actually happened or was done?
- Are metrics real and sourced? Placeholders flagged?
- Do labels and statuses match behaviour?

## Function
- Which interactions did you actually click, tab to or submit?
- Which checks ran: lint, types, tests, build?
- What did you not test? Say so.

## Finding format

| Severity | Where | Before | After | Why |
| --- | --- | --- | --- | --- |
| Blocker | Hero button | Link appears only on hover | Visible button at rest | Hover-only discovery fails keyboard and touch |

Cite the principle number from `design` in the Why column when one applies.
