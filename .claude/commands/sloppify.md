# Sloppify

Use the Sloppify editorial filter on the user's target: $ARGUMENTS

Review the provided copy, UI, component, screen, flow, or description for content and interface structure that looks polished but does not help the user.

Apply these tests:

1. Removal test: cut anything that costs the user no fact, decision, action, warning, or orientation.
2. Specificity test: rewrite generic lines with the actual object, state, user need, or consequence.
3. Duplication test: keep the clearest version of repeated headlines, subtitles, body lines, tooltips, CTAs, or sections.
4. Container test: flatten cards, panels, dividers, or disclosures that only decorate thin content.
5. Action test: make every button map to a distinct user action.
6. Evidence test: prefer visible facts, current state, next steps, constraints, or consequences.

Watch for:

- `not X, but Y` negative parallelism
- empty affirmation
- generic value claims
- app self-narration
- obvious state narration
- system apology copy
- count leaks
- hedge stacking
- intro and recap padding
- repeated triplets
- over-nested containers
- one-item sections
- duplicate CTAs
- buttons for passive information
- disclosure panels that justify weak content
- repeated metric representations
- decorative data cards

Avoid generic language such as `delve`, `intricate`, `tapestry`, `pivotal`, `underscore`, `foster`, `enhance`, `crucial`, `robust`, `seamless`, `boast`, `unlock`, `empower`, `leverage`, `showcase`, `groundbreaking`, `cutting-edge`, `game-changer`, `myriad`, `actionable`, `testament`, `cornerstone`, `innovative`, `vibrant`, and `transformative`.

Return:

1. **What to cut** - duplicated, generic, or decorative elements.
2. **What to rewrite** - before/after copy where useful.
3. **What to restructure** - cards, buttons, sections, or hierarchy.
4. **Clean version** - the tightened copy or UI structure.

Do not only criticize. Produce the sharper version.
