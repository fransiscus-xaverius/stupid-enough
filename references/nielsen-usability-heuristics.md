# 10 Usability Heuristics for User Interface Design (Nielsen, 1994)

## Citation
- Nielsen, J. (1994). Enhancing the explanatory power of usability heuristics. *Proceedings of the SIGCHI Conference on Human Factors in Computing Systems (CHI '94)*, 152–158. https://doi.org/10.1145/191666.191729
- Nielsen, J. (1994, updated). 10 Usability Heuristics for User Interface Design. Nielsen Norman Group. https://www.nngroup.com/articles/ten-usability-heuristics/

## Core idea
Jakob Nielsen's heuristics are broad, time-tested rules of thumb for interaction design. They are useful as evaluation checks to catch common usability problems. In the context of "stupid simple" UX, they are especially valuable for **keeping users informed, in control, and able to recover**.

## The 10 heuristics (summary)
1. **Visibility of system status**: keep users informed with timely, appropriate feedback.
2. **Match between system and the real world**: use familiar language, concepts, and conventions; present information in a natural order.
3. **User control and freedom**: provide clear exits, undo, redo, and cancel so users can recover from mistakes.
4. **Consistency and standards**: follow platform and product conventions; same things should look/behave the same way.
5. **Error prevention**: prevent problems before they happen (constraints, good defaults, confirmations only when truly risky/irreversible).
6. **Recognition rather than recall**: make options and information visible so users do not have to remember.
7. **Flexibility and efficiency of use**: support both novices and experts (shortcuts, accelerators) without complicating the default path.
8. **Aesthetic and minimalist design**: avoid irrelevant or rarely needed information competing with what matters.
9. **Help users recognize, diagnose, and recover from errors**: plain-language errors that explain the problem and suggest a fix.
10. **Help and documentation**: provide searchable, task-focused help when needed.

## UX implications (distinct to this principle set)
Use these as **validation checks**, with emphasis on safety and feedback:
- **Status visibility**: every action should have clear feedback (loading, success, failure, progress) within a reasonable time.
- **User control & freedom**: users can back out, cancel, or undo; no dead ends.
- **Error prevention and recovery**: design to avoid errors (smart defaults, constraints, inline validation) and make recovery easy (clear messages, actionable fixes, reversible actions).
- **Consistency**: consistent patterns and terminology reduce surprise and relearning (coordinate with conventions/clarity rules but verify explicitly).

> Note: Some heuristics overlap conceptually with other principles in this skill (e.g., #6 with memory/visibility, #8 with reducing extraneous load, #2/#4 with conventions and clarity). In the main skill, apply them as **non-duplicative checks**: use Nielsen primarily to verify status, control, and error handling; do not restate minimalism/chunking/conventions as separate Nielsen rules.

## Actionable checks
- [ ] Does the system clearly show what is happening now (idle, loading, saved, failed, progress)?
- [ ] Can users undo, cancel, or exit unwanted states easily?
- [ ] Are likely errors prevented by design (defaults, constraints, format hints, inline checks)?
- [ ] When errors occur, does the message state the issue plainly and tell the user how to fix it?
- [ ] Are similar elements and actions consistent in wording, placement, and behavior?

## External resources
- NN/g — 10 Usability Heuristics: https://www.nngroup.com/articles/ten-usability-heuristics/
- NN/g — How to Conduct a Heuristic Evaluation: https://www.nngroup.com/articles/how-to-conduct-a-heuristic-evaluation/
- Wikipedia — Heuristic evaluation: https://en.wikipedia.org/wiki/Heuristic_evaluation
