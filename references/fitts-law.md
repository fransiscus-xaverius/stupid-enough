# Fitts's Law (Fitts, 1954)

## Citation
- Fitts, P. M. (1954). The information capacity of the human motor system in controlling the amplitude of movement. *Journal of Experimental Psychology*, 47(6), 381–391. https://doi.org/10.1037/h0055392

## Core idea
The time required to move to and acquire a target depends on the distance to the target and the size of the target. In general: **closer and larger targets are faster and easier to hit**; smaller or farther targets take longer and are more error-prone.

A common formulation (Shannon form): *MT = a + b · log₂(D/W + 1)*, where *D* is distance to the target and *W* is target width/size along the axis of movement.

## Key nuances
- Target acquisition has phases: a fast ballistic movement toward the target and a slower corrective phase to land accurately; small targets increase correction time.
- On touch devices, "distance" includes thumb reach and hand posture; screen edges/corners can be easier to hit with a pointer on desktop because of constrained movement.
- Fitts's Law concerns motor/pointing performance, not decision time (Hick–Hyman) or cognitive understanding (Krug/Sweller).

## UX implications (distinct to this principle)
- **Make primary actions large**: important buttons/controls should have generous target size (commonly ≥ 44×44 CSS px for touch).
- **Ensure adequate spacing**: separate targets to prevent mis-taps/clicks.
- **Place key actions within easy reach**: on mobile, prioritize thumb-friendly zones (typically lower/central areas) for frequent primary actions; avoid placing critical controls only in hard-to-reach corners.
- **Reduce travel distance**: place related actions near the user's current focus/context; keep destructive or rare actions intentionally out of the fast path (but still accessible).
- **Prefer full-width/large hit areas** where appropriate (e.g., list rows, large cards) over tiny text links for primary interactions.

## Actionable checks
- [ ] Are primary interactive targets large enough (aim for ≥ 44×44 px touch targets, with comfortable padding)?
- [ ] Is there sufficient spacing between adjacent interactive elements to avoid accidental activation?
- [ ] Are the most frequent/primary actions placed in easy-to-reach areas for the device/context?
- [ ] Can hit areas be expanded (padding/invisible target) without changing visual layout?
- [ ] Are critical actions close to where the user’s attention already is at the moment of decision?

## External resources
- NN/g — Fitts’s Law and Its Applications in UX: https://www.nngroup.com/articles/fitts-law/
- Laws of UX — Fitts’s Law: https://lawsofux.com/fittss-law/
- Wikipedia — Fitts's law: https://en.wikipedia.org/wiki/Fitts%27s_law
