# Design QA

final result: passed

Reference direction: Product Design mockup option 2, "Facilitator Workshop Board".

Checks performed:
- Desktop viewport 1440 x 1024 renders as a three-column presentation/workshop board.
- Left agenda/timer, center nulägesövning, and right facilitator/säkra-val panel are visible without horizontal overflow.
- Mobile viewport 390 x 844 stacks content without horizontal overflow.
- Agenda navigation updates the slide counter, active step, and main presentation content.
- Previous/next buttons click through the seven workshop steps.
- Removed the former `Nulägescheck` module because it did not add enough value.
- Updated module timing to 0-5, 5-15, 15-27, 27-40, 40-55, 55-59, and 59-60 minutes.
- Added a concrete Copilot hands-on exercise with a safe fictitious HR case, copyable prompt, review checklist, and optional Copilot Chat agent instruction.
- Made imagery more prominent on the AI/ethics and Säkra val modules.
- 60-minute timer starts at 60:00, counts down, pauses, and can be reset.
- Existing PNG assets from `bilder/` are used in the relevant workshop steps and load lazily.
- Question cards update facilitator notes.
- Poll choices update active state.
- Safety guide drawer opens.
- Browser console has no JavaScript errors.

Remaining polish notes:
- The implementation uses lightweight inline SVG icons to keep this single-file workshop package dependency-free.
