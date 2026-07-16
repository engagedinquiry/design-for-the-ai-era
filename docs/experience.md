# EXPERIENCE.md

*Adapted from Design for the AI Era: Paradigm Shift — Persona, Screen, Context, Content, Time, and Trust chapters.*

---

## The design document is EXPERIENCE.md

Not an analogy. Not one implementation among several. Wherever the argument on `/design-document`, `/dimensions`, or `/polygon-grammar` refers to "the design document," it means this artifact, specifically — the governing decisions a designer makes about what an experience should be, for whom, and under what rules, written down before any build exists, in a form the build can execute from.

It is both input and output. It precedes the build and is updated by it. It is the designer's governing record and the AI's instruction set. It is readable by the designer, the client, the developer, and auditable at every point.

The document that never changes was never tested. The document that changes with every build is the document that is alive.

## What it contains

Every governing decision has a place here. Six sections, corresponding to the persona and the five dimensions:

**Persona** — the governing input. Named states, directed edges — not a target-audience description, but the authority the system consults at every transition. See `/polygon-grammar` for the full grammar this section is expressed in.

**Screen** — the governing ratio. Context-derived, not pixel-derived: the column unit, the space token, the type scale, the breakpoint behaviour. Change the ratio and the system changes coherently.

**Context** — the state stack. What each named state and each directed edge between states actually means for this system, specifically — not calculated, named.

**Content** — the selector. What content each context state receives, and at what level of resolution. One source record; the rules for assembling it per state live here, not duplicated per persona.

**Time** — decay rules. What the system holds, what it releases, on what motion grammar (dissolve for deepening, cut for pivoting) — deliberate decisions with real experiential consequences, made once, before any user arrives.

**Trust** — the audit rules. What a reviewer checks a build against. What's named, what's traceable, what makes a build accountable to the document rather than to whoever happened to prompt it.

## Skeleton

```markdown
---
version: 1.0
authored: [date]
governs: [system/product name]
---

# EXPERIENCE.md

## Persona
[The polygon grammar for this system. Named explicitly, not described generically —
see /polygon-grammar for the model this section applies.]

### Vertices (n core personas)
- [Persona A] — [what they came for, what they need]
- [Persona B] — [what they came for, what they need]
- [Persona C] — [what they came for, what they need]
[... one entry per core persona]

### Edges (directed — each pair is two distinct states, not one)
- [A → B] — [what this direction carries: e.g. curiosity becoming inquiry]
- [B → A] — [what the reverse carries: e.g. authority meeting encounter]
[... one pair per edge; direction changes the meaning, so both directions
of every edge must be named separately]

### Ambient
[The state where all personas are present, none dominant. What this
system does when a real person's position doesn't resolve to a single
vertex or edge.]

## Screen
[The governing ratio. Context-derived breakpoints: handheld/close/one-hand,
seated/medium/two-hands, ambient/long-distance/passive — or this system's
own equivalent set.]

## Context
[What each vertex and each directed edge, named above in Persona, actually
means for this system's layout, navigation, and available features. One
entry per state — not calculated, named.]

- [Vertex/Edge name] → [what the system does differently in this state]
[... one entry per vertex and per direction of every edge]

[What the state stack records as a person moves between these states —
the trace, not an identity.]

## Content
[The selector. What each named state receives, and at what resolution.
One source record; rules for assembly, not duplication.]

## Time
[Decay rules. What's held on deepening, what's released on retreat.
The motion grammar: dissolve vs. cut.]

## Trust
[What's auditable. What a build is checked against before release.
Who reviews, and what they're reviewing for.]
```

## The document is the handoff

The design document is the missing layer between intent and build. Without it, a build is an interpretation — small departures from intent that accumulate into drift. With it, a build is an execution: the document holds the intent, the build follows the document, the screens are the consequence.

The prompt, if one is used at all, is downstream of `EXPERIENCE.md` — generated from it, not a substitute for it. The more precise the document, the less an AI decides. The less an AI decides, the more the build reflects the governing principle someone actually authored.

---

*See `catenator.md`'s page for how this connects to `design.md` and `constitution.md`, `/polygon-grammar` for the persona grammar this document applies, and `/dimensions` for the full argument behind each of the five sections above.*
