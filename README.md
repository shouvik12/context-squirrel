# 🐿️ Context Squirrel

**Forget better.**

Generate project checkpoints that preserve what matters and discard what doesn't.

Most AI tools try to remember more.

Context Squirrel tries to remember less.

---

First real-world test:

```
3,150 tokens → 147 tokens

95% reduction.

Project survived.
```

---

## The Problem

Long AI conversations accumulate garbage.

Over time they collect:

- abandoned ideas
- rejected architectures
- resolved debates
- repeated explanations
- obsolete assumptions
- conversational drift

The result:

- higher token usage
- more repetition
- slower progress
- increased context pressure
- dead ideas getting resurrected

Eventually every long-running conversation starts carrying its own weight.

---

## The Thesis

Most conversation history is not project state.

A 500-turn conversation may contain:

- active signal
- historical baggage
- repeated reasoning
- dead-end explorations

The goal is not to preserve the conversation.

The goal is to preserve the project.

---

## Proof of Concept

Context Squirrel started from a simple question:

> Can a long conversation be reduced to its surviving project state without losing continuity?

First real-world test:

```
Before: 3,150 tokens
After:    147 tokens

Reduction: 95%
```

The resulting Clean SitRep retained enough information to continue the project in a fresh session.

No critical information was lost.

That result became the foundation for Context Squirrel.

---

## Why This Exists

Every token sent to an LLM costs money, attention, or context budget.

Whether you're using Claude, GPT, Gemini, or local models:

**More context ≠ Better context**

In long-running projects, the same ideas are discussed repeatedly. Old decisions remain in context long after they stop being useful. Resolved debates continue consuming tokens. Abandoned ideas continue influencing future responses.

Context Squirrel extracts what still matters and leaves the rest behind.

---

## Install

1. Download `clean-sitrep.md` or `authentic-sitrep.md`
2. Create a new Claude Project
3. Add the file to the project's instructions
4. Start a conversation inside that project
5. When needed, ask:

```
clean sitrep
```

or

```
authentic sitrep
```

6. Copy the generated SitRep into a fresh conversation to continue with a smaller context footprint

---

## Two Modes

### Authentic SitRep

Preserve continuity.

Use when handing off a project, moving to a new session, or archiving project state.

Keeps: project identity, decision history, rationale, current state, open loops.

```
ANCHOR
DECISIONS
CURRENT STATE
OPEN LOOPS
TAIL
```

> What happened and why?

---

### Clean SitRep

Preserve focus.

Use when starting a fresh chat, reducing context bloat, or recovering project clarity.

Keeps: project identity, surviving decisions, current truth, open loops, negative memory.

```
ANCHOR
SURVIVING DECISIONS
CURRENT STATE
OPEN LOOPS
NEGATIVE MEMORY
TAIL
```

> What still matters?

---

## Negative Memory

The most important feature.

Most memory systems ask:

> What should be remembered?

Context Squirrel also asks:

> What should stay forgotten?

Example:

```
Do not revisit MCP-first architecture
unless browser extension assumptions change.

Do not revisit aggressive lossy compression
unless lossless opportunities are exhausted.

Do not build Phase 2
before validating Phase 1.
```

Negative Memory prevents known dead ends from continuously reappearing. It records not only what survived — it records what was intentionally rejected.

---

## Token Savings

Context Squirrel is not a token optimizer.

It is a context optimizer.

Token savings are a consequence of removing conversational garbage.

First real-world test:

```
Before: 3,150 tokens
After:    147 tokens

Reduction: 95%
```

The compressed version preserved project identity, active decisions, current state, open loops, and known dead ends — while removing abandoned ideas, resolved debates, repeated explanations, and conversational drift.

Larger projects often contain significantly more removable context.

**Keep the signal. Discard the noise.**

---

## Never-Ending Conversations

Instead of carrying a massive conversation forever:

```
Conversation
      ↓
Clean SitRep
      ↓
Fresh Session
      ↓
Continue
```

The conversation becomes disposable. The project state survives.

A project may span hundreds of turns across multiple sessions while carrying only the information that still matters.

---

## Philosophy

Context Squirrel is not:

- memory
- retrieval
- RAG
- vector search
- a second brain
- a knowledge base

Context Squirrel is:

```
State Extraction
+
Selective Forgetting
+
Project Continuity
```

Most AI tooling focuses on remembering more.

Context Squirrel focuses on forgetting correctly.

---

## Future Direction

- Browser extensions
- Context health analysis
- Dead-end detection
- State diff generation
- Long-session workflow automation

The core idea remains unchanged: extract the state, preserve the signal, discard the noise.

---

## Core Idea

Remember the project.

Forget the conversation.

---

**Forget better.** 🐿️
