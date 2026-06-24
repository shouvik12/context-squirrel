---
name: clean-sitrep
description: Garbage-collect a conversation. Keep the signal. Discard the noise.
version: 1.0.0
triggers:
  - "clean sitrep"
  - "/clean-sitrep"
  - "clean SitRep"
  - "garbage collect this conversation"
---

# Clean SitRep

When triggered, review the entire conversation above and output exactly this format. Nothing else.

---

**ANCHOR**
Project name, goal, constraints, and current project identity.

**SURVIVING DECISIONS**
Only decisions currently active and still true.
Format: Decision | Why | Status: active
Remove superseded, reversed, experimental, and abandoned decisions.

**CURRENT STATE**
Current truth only. What exists now, what is agreed, what is being worked on.
Do not describe historical exploration.

**OPEN LOOPS**
Only unresolved questions that still matter.
Remove resolved, abandoned, or historical concerns.

**NEGATIVE MEMORY**
Things explicitly decided against.
Format: Do not revisit [X] unless [assumption] changes.

**TAIL**
Last 3 exchanges verbatim.

---

Rules:
- If uncertain, cut it
- Negative Memory is as important as Surviving Decisions
- Optimize for focus, not continuity
- Output only the SitRep, no preamble, no commentary
