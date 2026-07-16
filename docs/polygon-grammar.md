# Polygon-grammar

*Adapted from Design for the AI Era: Paradigm Shift — Persona chapter.*

---

## Cogitasti, ergo sum

In practice, a persona is usually a type wearing a name. Hours of research producing a slide — a stock photograph, an occupation, a list of frustrations, an assumed aspiration. Presented once. Filed. The sprint begins, and the grid makes the decisions without it.

The persona was invented to get the user into the room when the user wasn't there — a placeholder built from real observation, a way of keeping an actual audience visible during decisions that would otherwise be made for nobody in particular. It started honestly. It became a deliverable, then a formality, then — in AI systems trained on the aggregate of every user who ever interacted with anything — invisible entirely. A prediction with no name, no photograph, nothing on a wall to argue with.

**The persona governs, or it decorates. There is no middle position.**

## What a polygon grammar is

A polygon grammar is what putting the persona to work actually looks like, structurally.

Most systems assume one persona, or an average of several, producing one screen — a single, compromised design meant to serve everyone adequately and no one precisely. A polygon grammar starts from a different premise: a system usually has more than one real persona, each one expecting a genuinely different screen — not a variation on the same layout, but a different set of governing decisions entirely, because what a Visitor needs and what a Researcher needs are not the same problem with different content. They are different problems.

A polygon grammar names each of those personas as a vertex, and treats the space between them as real territory rather than empty space to be smoothed over. Every position in that space — not just the vertices themselves — corresponds to a specific, nameable state, and every state gets its own governing decisions: its own layout, its own content rules, its own screen. The grammar is what makes it possible to hold many distinct personas, and the many distinct screens each one requires, inside one coherent system without collapsing them into a single average.

## The physical proof

A physical museum does not design for the average visitor. It designs for several distinct people, and the building reflects every one of them — a visitor wants orientation and theatre; a researcher wants density and a quiet place to sit; a media enthusiast wants presence, not record. Architecture solves this without anyone having to name it: service corridors, reading rooms, separate paths that never force one visitor's needs onto another's experience.

A digital system can't solve this with architecture. It has to do it with governance.

## The geometry of intent

Three personas. Three distinct modes of engagement — Visitor, Researcher, Media enthusiast. But people don't arrive with a single, fixed intent. They arrive curious and become focused. They arrive for one thing and stay for another.

Place the three personas at the vertices of a triangle. The space between them is not empty — it is the territory of transition. The edges between them name something real, and **the direction of the edge matters.**

Visitor moving toward Researcher is not the same as Researcher moving toward Visitor. The first carries curiosity into depth — someone who came to look and stayed to read. The second carries authority into encounter — someone who came with a question and is now browsing more broadly. Same edge. Opposite intent. Different experience. Different governing decisions.

## P(3) — the ten states

| | |
|---|---|
| **Core (3)** | Visitor · Researcher · Media enthusiast |
| **Intermediates (6)** | Visitor→Researcher · Researcher→Visitor · Visitor→Media · Media→Visitor · Researcher→Media · Media→Researcher |
| **Ambient (1)** | All three present, none dominant |

Each intermediate state names a specific, real transition — not a blend, a genuinely distinct posture:

- **Visitor → Researcher** — curiosity becoming inquiry
- **Researcher → Visitor** — authority meeting encounter
- **Visitor → Media** — encounter becoming immersion
- **Media → Visitor** — immersion complete, now browsing
- **Researcher → Media** — inquiry becoming visual
- **Media → Researcher** — image found, now seeking context

Each state is named, not calculated. The designer assigns layouts and governing rules to named slots. The underlying coordinate math — barycentric position within the triangle — is internal to the system. The designer never sees it, and doesn't need to.

**The name is the governing act.** Naming is the decision that this specific combination of personas, in this system, for this audience, means this specific encounter. The name holds the designer accountable. The design document holds the name. The system executes the document.

## The state stack

The persona does not reset between visits. It is a journey. A stateless page discards that journey with every load; a governed system holds it — not as a record of who the user is, but as a trace of what they did, where they went, what they were looking for when they crossed from one state into another.

**The trace is the user.**

With more than three personas, the same geometry generalises — P(n) rather than P(3), more vertices, more named edges, the same governing logic. There is no limit to how many personas a system can anchor, as long as each transition is named deliberately rather than left to calculate itself.

## Semper sum

*I always am — not in a deck that nobody updates. In the design document that precedes the grid. In the system that executes the document. In every screen the user will ever see.*

---

*See `/governance` for how a real person's position within this grammar is sensed at request time, and `/prism` for how that position becomes a specific, revealed output.*
