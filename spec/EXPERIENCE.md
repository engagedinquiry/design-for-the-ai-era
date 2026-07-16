---
version: 1.0
authored: [date]
governs: [system/product name]
---

# EXPERIENCE.md

<!--
This is the design document. See docs/design-document-is-the-product.md for
what this file is and why it matters, and docs/methodology.md for the full
argument behind it. This file is the artifact itself — fill it in.
-->

## Persona

<!-- The polygon grammar for this system. See docs/polygon-grammar.md. -->

### Vertices (n core personas)
- [Persona A] — [what they came for, what they need]
- [Persona B] — [what they came for, what they need]
- [Persona C] — [what they came for, what they need]

### Edges (directed — each pair is two distinct states, not one)
- [A → B] — [what this direction carries]
- [B → A] — [what the reverse carries]

### Ambient
[The state where all personas are present, none dominant. What this system
does when a real person's position doesn't resolve to a single vertex or edge.]

## Screen

<!-- See docs/dimensions.md — Screen -->

[The governing ratio. Context-derived breakpoints, not device-derived —
handheld/close/one-hand, seated/medium/two-hands, ambient/long-distance/passive,
or this system's own equivalent set.]

## Context

<!-- See docs/dimensions.md — Context -->

[What each vertex and each directed edge, named above in Persona, actually
means for this system's layout, navigation, and available features.]

- [Vertex/Edge name] → [what the system does differently in this state]

[What the state stack records as a person moves between these states.]

## Content

<!-- See docs/dimensions.md — Content -->

[The selector. What each named state receives, and at what resolution.
One source record; rules for assembly, not duplication.]

## Time

<!-- See docs/dimensions.md — Time -->

[Decay rules. What's held on deepening, what's released on retreat.
The motion grammar: dissolve vs. cut.]

## Trust

<!-- See docs/dimensions.md — Trust -->

[What's auditable. What a build is checked against before release.
Who reviews, and what they're reviewing for.]
