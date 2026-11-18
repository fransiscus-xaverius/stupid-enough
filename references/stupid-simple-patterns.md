# "Stupid Simple" UI Patterns and Examples

These examples translate cognitive research into concrete interface patterns. Each pattern includes a before/after contrast and an extracted rule.

## 1. Single-question flow (Typeform / Lemonade)

- **Traditional complex flow**: a long form (e.g., 25 fields for insurance or a survey) shown all at once, causing overwhelm and abandonment.
- **Ultra-simple flow**: one question per screen with large, tappable answer options and automatic/clear progression to the next step.
- **Why it works**: reduces intrinsic cognitive load per screen, limits immediate decisions, and keeps attention on one task.
- **Extracted rule**: **Never present a long, dense form by default.** Prefer one question or at most a very small, tightly related group per step (target: 1–3 inputs per screen). Convert long forms into a linear, step-by-step flow with clear progress.

## 2. Zero-chrome entry (Google Search / Hemingway Editor)

- **Traditional complex UI**: a crowded start surface with sidebars, feeds, widgets, and multiple competing menus.
- **Ultra-simple UI**: a blank or near-blank canvas with a single focal point (e.g., one search box, one immediate writing area).
- **Why it works**: removes extraneous load and competing choices so the primary action is unmistakable.
- **Extracted rule**: **Make the primary task the hero.** Hide secondary navigation, settings, and toolbars behind an optional drawer/menu until the user completes or explicitly requests secondary actions.

## 3. Smart defaults & one-tap recovery (Gmail / Uber)

- **Traditional complex flow**: require users to manually enter predictable information (e.g., current location) or interrupt them with irreversible "Are you sure?" confirmation modals.
- **Ultra-simple flow**: auto-detect or pre-fill predictable inputs so the user provides only what is unique (e.g., destination), and execute actions immediately with a temporary, reversible **Undo** when possible.
- **Why it works**: reduces effort and decision points, prevents errors by default, and preserves user control without blocking flow.
- **Extracted rule**: **Pre-fill predictable inputs and prefer reversible actions over blocking confirmations.** Use smart defaults, auto-detection, and undo toasts/snackbars instead of modal confirmation dialogs when the action can be safely reversed.

## Applying the patterns
- Start from the user's primary job-to-be-done; design the first screen around that single action.
- Default to fewer fields, fewer choices, and fewer visible controls; reveal complexity progressively.
- Automate what the system can know; ask the user only for what the system cannot know.
- When in doubt, choose the path that is easier to scan, easier to tap, and easier to undo.
