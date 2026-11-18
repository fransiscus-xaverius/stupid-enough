---
name: Stupid Enough
description: Design and review "stupid simple" UX using non-overlapping rules grounded in cognitive research (cognitive load, choice, target ergonomics, chunking, clarity, and safety).
---

# Stupid Enough UX

Use this skill to design, simplify, or review interfaces so they are immediately understandable and easy to complete with minimal thought. Apply it to flows, screens, forms, navigation, copy, interaction design, and UX critiques.

## Goal

Produce UX that is **stupid simple**: the user can see what this is, choose what to do, do it easily, and recover safely without unnecessary thinking, memory, or effort.

## How to use

1. **Identify the primary job-to-be-done** for the screen/flow (the one thing the user came to do now).
2. **Trace the flow**: entry → required inputs/decisions → outcome → loading/empty/error/success states.
3. **Apply the six principles below in order**. Each principle has a distinct scope; do not restate the same rule under multiple principles.
4. **Use the concrete patterns** in `references/stupid-simple-patterns.md` to translate principles into layouts.
5. **Run the validation checklist** before finalizing and call out any intentional tradeoffs.

## Six non-overlapping principles

Each rule belongs to exactly one principle. If a concern seems related to two principles, assign it by scope:
- **What is shown / how much complexity** → Principle 1
- **How many choices/decisions** → Principle 2
- **How easy to physically target** → Principle 3
- **How information is grouped/remembered** → Principle 4
- **How obvious/comprehensible it is** → Principle 5
- **How status/control/errors are handled** → Principle 6

### 1) Cut cognitive noise
**Source:** Cognitive Load Theory (Sweller, 1988) — `references/cognitive-load-sweller-1988.md`  
**Scope:** Extraneous elements and intrinsic complexity per view/step. Minimize waste; manage necessary complexity.

**Rules**
- Remove anything that does not help the user complete the current task (decorative clutter, redundant copy, irrelevant options surfaced too early).
- Give each screen/view **one primary purpose** and one focal point.
- Manage intrinsic complexity by splitting complex work into ordered, single-purpose steps; show only what is needed now.
- Keep related instructions and controls together to avoid split attention.
- Default to a calm, sparse layout; reveal advanced detail progressively.

**Checks**
- [ ] Can any element be removed without harming completion? Remove it.
- [ ] Is the screen focused on one job?
- [ ] Is a complex flow broken into steps instead of a dense all-at-once surface?

### 2) Limit decisions
**Source:** Hick–Hyman Law (Hick, 1952; Hyman, 1953) — `references/hick-hyman-law.md`  
**Scope:** Number and structure of choices/actions presented at once. Reduce decision time and deliberation.

**Rules**
- Provide **exactly 1 primary action** per view/step and at most **2 secondary actions**, visually de-emphasized.
- Avoid presenting many competing options; defer non-essential choices behind progressive disclosure ("More", advanced, later step).
- Break multi-decision tasks into a sequence where each step asks for one decision.
- When many options are unavoidable, categorize or structure them so users choose a group before a specific item; highlight a sensible recommended/default path where appropriate.

**Checks**
- [ ] Is there one clear primary action and ≤ 2 secondary actions?
- [ ] Are uncommon options deferred rather than shown upfront?
- [ ] Does each step require only one key decision?

### 3) Make actions easy to hit
**Source:** Fitts's Law (Fitts, 1954) — `references/fitts-law.md`  
**Scope:** Motor/pointing ergonomics — target size, spacing, and placement. Make intended actions fast and accurate.

**Rules**
- Make primary interactive targets large (aim for **≥ 44×44 px** touch targets with comfortable padding/hit area).
- Provide sufficient spacing between targets to prevent mis-taps/mis-clicks.
- Place frequent/primary actions in easy-to-reach areas for the context (e.g., thumb-friendly zones on mobile; near the user's current focus).
- Keep related actions close to where the decision is made; expand hit areas where helpful without adding visual noise.

**Checks**
- [ ] Are primary targets ≥ 44×44 px with adequate spacing?
- [ ] Are frequent actions placed within easy reach?
- [ ] Are hit areas large enough even if the visible label/icon is small?

### 4) Chunk and group
**Source:** Miller (1956), informed by later chunking research — `references/miller-magical-number-seven.md`  
**Scope:** Organization of information into meaningful units for scanning and (when necessary) recall. Structure, don't arbitrarily truncate.

**Rules**
- Group related items into small, meaningful clusters (aim for **~3–5 items per cluster** where practical) with clear labels/headings and spacing.
- Chunk long strings/data (phone numbers, codes, IDs, card numbers) into familiar segments for readability.
- Minimize cross-step memory burden: if users must remember information between steps, keep it visible or reduce it to a few chunks.
- **Recognition ≠ recall:** do not cap visible, recognizable content (e.g., a visible menu) to 7 items solely due to memory limits; use grouping and hierarchy instead.

**Checks**
- [ ] Are related elements organized into labeled clusters of manageable size?
- [ ] Is long formatted data chunked?
- [ ] Is memory across steps minimized or externalized on screen?

### 5) Make it self-evident
**Source:** Don't Make Me Think (Krug, 2000) — `references/dont-make-me-think-krug.md`  
**Scope:** Comprehension, scanning, conventions, and obviousness. Users should not have to puzzle over meaning or next steps.

**Rules**
- Make the screen's purpose and the next action obvious within seconds (self-evident or self-explanatory).
- Establish a clear visual hierarchy so users can scan: what matters most, what is related, and what to do first.
- Use plain, specific labels and familiar conventions (platform/web patterns, standard icon meanings, expected locations/behaviors); avoid jargon and clever-but-unclear wording.
- Keep wording, placement, and behavior consistent for similar elements and actions so users do not have to relearn.
- Make interactive elements look interactive and support satisficing: the first reasonable option should be the right/easiest one to notice.
- Write for scanning: concise headings, front-loaded keywords, short blocks, no needless words.

**Checks**
- [ ] Can a first-time user identify purpose and next step at a glance?
- [ ] Are labels/actions self-explanatory, convention-aligned, and consistent?
- [ ] Does visual hierarchy make the primary path unmistakable?

### 6) Keep users safe and informed
**Source:** 10 Usability Heuristics (Nielsen, 1994) — `references/nielsen-usability-heuristics.md`  
**Scope:** System feedback, user control/freedom, and error prevention/recovery. (Other Nielsen concerns are intentionally handled by Principles 1, 4, and 5 to avoid overlap.)

**Rules**
- **Status visibility:** always show what is happening (idle, loading/progress, success, failure) with timely, clear feedback for every meaningful action.
- **Control and freedom:** provide easy undo, cancel, back, or exit; avoid dead ends and irreversible traps.
- **Prevent errors:** use smart defaults, constraints, format hints, and inline validation to stop likely mistakes before submission.
- **Recover clearly:** prefer reversible actions (e.g., undo) over blocking confirmations when safe; when errors occur, explain the issue in plain language and state how to fix it.

**Checks**
- [ ] Does every action produce clear feedback/status?
- [ ] Can users undo/cancel/exit easily?
- [ ] Are predictable inputs pre-filled/defaulted and likely errors prevented?
- [ ] Are error states plain, specific, and actionable?

## Concrete patterns (apply where relevant)
- **Single-question flow:** convert long forms into step-by-step screens; aim for 1 question or 1–3 tightly related inputs per step with clear progress. (`references/stupid-simple-patterns.md`)
- **Zero-chrome entry:** lead with one focal action; hide secondary navigation/settings until needed. (`references/stupid-simple-patterns.md`)
- **Smart defaults & one-tap recovery:** auto-detect/pre-fill predictable inputs; prefer immediate action + temporary undo over blocking confirmation modals when reversible. (`references/stupid-simple-patterns.md`)

## Output expectations when using this skill
When asked to design or review UX, provide:
- A brief statement of the **primary user goal** and the simplified flow.
- The proposed screen/step structure (or critique) with specific UI decisions.
- How the six principles are satisfied (and any tradeoffs/constraints).
- Concrete copy/layout/interaction recommendations (e.g., primary CTA, field grouping, defaults, states, undo behavior), not just abstract advice.

## References (local)
- `references/cognitive-load-sweller-1988.md` — Sweller (1988), intrinsic/extraneous/germane load, simplification and sequencing.
- `references/hick-hyman-law.md` — Hick (1952), Hyman (1953), choice count and decision time.
- `references/fitts-law.md` — Fitts (1954), target size, distance, reach.
- `references/miller-magical-number-seven.md` — Miller (1956), chunking and memory limits (recognition vs recall).
- `references/dont-make-me-think-krug.md` — Krug (2000), scanning, satisficing, self-evident design and conventions.
- `references/nielsen-usability-heuristics.md` — Nielsen (1994/updated), status, control, error prevention/recovery, and heuristic checks.
- `references/stupid-simple-patterns.md` — Single-question flow, zero-chrome entry, smart defaults & undo.
