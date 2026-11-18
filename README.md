# Stupid Enough

An agent skill for designing and planning **stupid simple UX** grounded in human cognitive research.

`stupid-enough` helps turn complex interfaces into clear, low-friction flows by applying a small set of non-overlapping, research-backed rules. It is intended for UX design, simplification, review, and planning work (flows, screens, forms, navigation, copy, interaction states).

## What's in this repo

- [`SKILL.md`](./SKILL.md) — the skill definition and operating instructions
- [`references/`](./references/) — source summaries and pattern notes referenced by the skill
  - [`cognitive-load-sweller-1988.md`](./references/cognitive-load-sweller-1988.md)
  - [`hick-hyman-law.md`](./references/hick-hyman-law.md)
  - [`fitts-law.md`](./references/fitts-law.md)
  - [`miller-magical-number-seven.md`](./references/miller-magical-number-seven.md)
  - [`dont-make-me-think-krug.md`](./references/dont-make-me-think-krug.md)
  - [`nielsen-usability-heuristics.md`](./references/nielsen-usability-heuristics.md)
  - [`stupid-simple-patterns.md`](./references/stupid-simple-patterns.md)

## How the skill works

The skill guides an agent to:
1. Identify the **primary job-to-be-done** for the screen/flow.
2. Trace the flow: entry → decisions/inputs → outcome → loading/empty/error/success states.
3. Apply **six non-overlapping principles** (each with a distinct scope).
4. Use concrete "stupid simple" patterns to translate principles into UI decisions.
5. Validate the result with explicit checks and call out tradeoffs.

## Six non-overlapping principles

| # | Principle | Source | Scope (distinct) |
|---|-----------|--------|------------------|
| 1 | **Cut cognitive noise** | Cognitive Load Theory (Sweller, 1988) | Extraneous elements and intrinsic complexity per view/step |
| 2 | **Limit decisions** | Hick–Hyman Law (Hick, 1952; Hyman, 1953) | Number/structure of choices and actions at once |
| 3 | **Make actions easy to hit** | Fitts's Law (Fitts, 1954) | Target size, spacing, reach/placement (motor ergonomics) |
| 4 | **Chunk and group** | Miller (1956), chunking research | Information grouping and cross-step memory burden (recognition ≠ recall) |
| 5 | **Make it self-evident** | Don't Make Me Think (Krug, 2000) | Comprehension, scanning, conventions, labels, consistency, obvious next step |
| 6 | **Keep users safe and informed** | Nielsen's 10 Usability Heuristics (1994) | System status, user control/freedom, error prevention and recovery |

Rules are assigned to exactly one principle by scope to avoid overlap (e.g. minimalism → noise/load, choice count → decisions, conventions/consistency → self-evidence, feedback/undo/errors → safety).

## Concrete patterns included

- **Single-question flow** (e.g. Typeform, Lemonade): one question or 1–3 tightly related inputs per step; convert long forms into a linear flow with clear progress.
- **Zero-chrome entry** (e.g. Google Search, Hemingway Editor): lead with one focal primary action; hide secondary navigation/settings until needed.
- **Smart defaults & one-tap recovery** (e.g. Gmail, Uber): pre-fill/auto-detect predictable inputs; prefer immediate action + temporary undo over blocking confirmations when reversible.

See [`references/stupid-simple-patterns.md`](./references/stupid-simple-patterns.md).

## Using this skill

- **OpenCode / compatible agents:** place or reference this repository so the agent can discover `SKILL.md` (directory form with `references/` alongside it). Invoke/load the skill when designing or reviewing UX.
- **Manual use:** read [`SKILL.md`](./SKILL.md) and the files in [`references/`](./references/) as a checklist and design guide.

When applied, the skill expects concrete output: primary user goal, simplified flow/screen structure, specific UI decisions, how the six principles are satisfied, and actionable recommendations (CTA, fields, grouping, defaults, states, undo/error behavior), including tradeoffs.

## Sources used in creating this skill

### Foundational research and texts
- **Cognitive Load Theory** — Sweller, J. (1988). *Cognitive load during problem solving: Effects on learning.* Cognitive Science, 12(2), 257–285. https://doi.org/10.1207/s15516709cog1202_4  
  Also informed by: Sweller, J., van Merriënboer, J. J. G., & Paas, F. (1998). *Cognitive architecture and instructional design.* Educational Psychology Review, 10, 251–296.
- **Hick–Hyman Law** — Hick, W. E. (1952). *On the rate of gain of information.* Quarterly Journal of Experimental Psychology, 4(1), 11–26. https://doi.org/10.1080/17470215208416600  
  Hyman, R. (1953). *Stimulus information as a determinant of reaction time.* Journal of Experimental Psychology, 45(3), 188–196. https://doi.org/10.1037/h0056940
- **Fitts's Law** — Fitts, P. M. (1954). *The information capacity of the human motor system in controlling the amplitude of movement.* Journal of Experimental Psychology, 47(6), 381–391. https://doi.org/10.1037/h0055392
- **The Magical Number Seven, Plus or Minus Two** — Miller, G. A. (1956). *The magical number seven, plus or minus two: Some limits on our capacity for processing information.* Psychological Review, 63(2), 81–97. https://doi.org/10.1037/h0043158  
  Chunking/memory-capacity nuance: Cowan, N. (2001). *The magical number 4 in short-term memory: A reconsideration of mental storage capacity.* Behavioral and Brain Sciences, 24(1), 87–114.
- **Don't Make Me Think** — Krug, S. (2000). *Don't Make Me Think: A Common Sense Approach to Web Usability.* New Riders. (later revised editions). https://sensible.com/dont-make-me-think/
- **10 Usability Heuristics for User Interface Design** — Nielsen, J. (1994). *Enhancing the explanatory power of usability heuristics.* CHI '94, 152–158. https://doi.org/10.1145/191666.191729  
  Nielsen Norman Group article (updated): https://www.nngroup.com/articles/ten-usability-heuristics/

### Design references and summaries consulted
- Laws of UX — Hick’s Law: https://lawsofux.com/hicks-law/
- Laws of UX — Fitts’s Law: https://lawsofux.com/fittss-law/
- Laws of UX — Miller’s Law: https://lawsofux.com/millers-law/
- Nielsen Norman Group — Fitts’s Law and Its Applications in UX: https://www.nngroup.com/articles/fitts-law/
- Nielsen Norman Group — 10 Usability Heuristics for User Interface Design: https://www.nngroup.com/articles/ten-usability-heuristics/
- Nielsen Norman Group — Chunking: https://www.nngroup.com/articles/chunking/
- Interaction Design Foundation (IxDF) — Don’t Make Me Think, key learning points: https://www.interaction-design.org/literature/article/don-t-make-me-think-key-learning-points-for-ux-design-for-the-web
- Wikipedia pages for contextual summaries: [Cognitive load](https://en.wikipedia.org/wiki/Cognitive_load), [Hick's law](https://en.wikipedia.org/wiki/Hick%27s_law), [Fitts's law](https://en.wikipedia.org/wiki/Fitts%27s_law), [The Magical Number Seven, Plus or Minus Two](https://en.wikipedia.org/wiki/The_Magical_Number_Seven,_Plus_or_Minus_Two), [Don't Make Me Think](https://en.wikipedia.org/wiki/Don%27t_Make_Me_Think)

### Example products/patterns referenced
- **Single-question flow:** Typeform, Lemonade (one question per step, clear progression)
- **Zero-chrome entry:** Google Search, Hemingway Editor (single focal primary action)
- **Smart defaults & one-tap recovery:** Gmail (Undo), Uber (auto-detected pickup / minimal required input)

Local synthesized notes for all of the above are in [`references/`](./references/).

## License

MIT — see [`LICENSE`](./LICENSE).
