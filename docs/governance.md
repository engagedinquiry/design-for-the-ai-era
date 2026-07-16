# /governance

*Register: Narrative, leading into the technical detail Prism and the spec build on.*

---

## What governing means here

A governed system is one where the decisions precede the build, are written down, and constrain everything generated afterward — rather than decisions being made implicitly, differently, every time something is generated.

This applies to any Catenator-governed system, not only published content. A product, an app, a design system — anything a design document specifies — is governed the same way. What follows is general on purpose.

## The governing document

The design document is both input and output. It precedes the build and is updated by it. It is the record of what the governing principle produces before anyone experiences it — written before the build, updated by it, readable by the designer, the client, the developer. Auditable at every point.

The document that never changes was never tested. The document that changes with every build is the document that is alive.

## The governing persona

Persona is the governing input that shapes everything else a design document specifies. It is not a target-audience description, and it is not a single imagined average user. It is the authority the system consults at every transition — the reason a decision was made one way rather than another, stated once, before the build exists to test it.

Where a target-audience persona describes who a product is *for*, a governing persona describes who the system answers *to* — a distinction that matters once a system starts producing different outputs for different people. Without it, that variation is guesswork. With it, every variation traces back to a decision someone actually made.

## The governing line

At the level of an individual piece — one screen, one document, one published piece of work — the governing document's principle is expressed as a governing line: one sentence naming what this specific piece is doing and who it assumes its audience to be.

A brief that disappears after handoff was never really governing anything. A governing line is not a memory of what was decided once; it is a live constraint that can be tested against the actual output at any point. It is the smallest unit of governance — small enough to write for one piece, precise enough to hold that piece accountable to the larger document it descends from.

## The log — a governance requirement, not a Prism feature

A governed system needs to know, at the moment of a request, where a real person currently sits within the persona grammar the design document defined. That requires some mechanism for sensing intent, depth, and history — a log, in the general sense.

This standard requires that such a mechanism exist. It does not prescribe how it is implemented. What it does require:

- **Local.** The sensing happens on the person's own device, not on a server.
- **Never transmitted.** What is sensed stays where it was sensed. No behavioural history leaves the device as a condition of the system working correctly.
- **Honest to the grammar.** Whatever the log determines must map cleanly onto the persona states the design document actually defined — it cannot invent positions the document didn't specify.

Beyond those three requirements, the implementation is not this standard's concern. A system can build its own log, adapt an existing one, or use a third-party implementation — provided it satisfies what's above. What matters to Prism is only that the log supplies intent and context state as an input; how it does so is a governance decision made separately from the rendering mechanism itself.

## Where this leads

The governing document defines what's possible. The governing persona and governing line state, at the system level and the piece level, who that possibility is being decided for. The log determines, at request time, where a specific person actually is. **Prism** then reveals what was already true for that position — covered in full at `/prism`.

---

*See `/design-document` for the full argument, `/polygon-grammar` for the persona state-space itself, and `/prism` for how a governed position becomes a specific output.*
