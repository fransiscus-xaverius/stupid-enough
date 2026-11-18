# Hick–Hyman Law (Hick, 1952; Hyman, 1953)

## Citation
- Hick, W. E. (1952). On the rate of gain of information. *Quarterly Journal of Experimental Psychology*, 4(1), 11–26. https://doi.org/10.1080/17470215208416600
- Hyman, R. (1953). Stimulus information as a determinant of reaction time. *Journal of Experimental Psychology*, 45(3), 188–196. https://doi.org/10.1037/h0056940

## Core idea
Decision/reaction time increases as the number and complexity of available choices increases (commonly modeled as a logarithmic relationship: *RT = a + b · log₂(n + 1)* for *n* equiprobable choices). More options mean more time and effort to decide.

## Key nuances
- The increase is not simply linear; adding options to an already small set has a noticeable impact, and large unstructured sets create significant friction and fatigue.
- Structure matters: categorizing options and using familiar orderings can reduce effective decision effort.
- Hick–Hyman describes choice/decision time, not motor movement time (see Fitts's Law) and not memory span (see Miller).

## UX implications (distinct to this principle)
- **Limit choices per view**: prefer one clear primary action and a small number of secondary options.
- **Progressive disclosure**: reveal advanced or less common options only when requested, instead of presenting everything upfront.
- **Break decisions into steps**: use wizards/step flows so each screen asks for one decision at a time.
- **Highlight the recommended path**: make the default or most common choice obvious to reduce deliberation.
- **Categorize when many options are necessary**: group and label options so users choose a category before a specific item.

## Actionable checks
- [ ] Is there exactly one primary action on this screen/view?
- [ ] Are secondary actions limited (aim for ≤ 2) and visually de-emphasized?
- [ ] Can any options be deferred behind "More", an advanced section, or a later step?
- [ ] Is a sensible default or recommended option provided where appropriate?
- [ ] Are long option sets categorized or searchable instead of shown as one flat list?

## External resources
- Laws of UX — Hick’s Law: https://lawsofux.com/hicks-law/
- Wikipedia — Hick's law: https://en.wikipedia.org/wiki/Hick%27s_law
- IxDF — Hick’s Law: https://www.interaction-design.org/literature/topics/hick-s-law
