---
name: authentic-sitrep
description: Preserve everything future Claude will need to continue without losing context.
version: 1.0.0
triggers:
  - "authentic sitrep"
  - "/authentic-sitrep"
  - "authentic SitRep"
  - "preserve this conversation"
  - "continue in new chat"
---

# Authentic SitRep

When triggered, review the entire conversation above and output exactly this format. Nothing else.

---

**ANCHOR**
Project name, goal, constraints, and current project identity.

**DECISIONS**
All decisions, active or superseded.
Format: Decision | Why | Status (active/superseded/reversed)

**CURRENT STATE**
Where the project is now and how it got here.
What exists, what was tried and changed, what is being worked on now.

**OPEN LOOPS**
All unresolved questions, including ones that stalled.

**TAIL**
Last 5 exchanges verbatim.

---

Rules:
- Preserve rationale even if verbose
- When in doubt, keep it
- Optimize for continuity, not focus
- Output only the SitRep, no preamble, no commentary
