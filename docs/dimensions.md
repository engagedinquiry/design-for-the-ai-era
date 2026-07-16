# /dimensions


*Adapted from Design for the AI Era: Paradigm Shift — Screen, Context, Content, Time, and Trust chapters. Persona is the governing input; these five are what it governs.*

---

Five dimensions of digital experience. Not tied to the browser, the pixel, or the device — the dimensions of any governed communication, whatever form the delivery takes. Each one is a decision a design document makes before a build exists to test it.

## Screen

*Adapted from Design for the AI Era: Paradigm Shift — Screen chapter.*

**What it governs:** the rectangle itself — not as a rendering target, but as a governed surface with an obligation to the person in front of it.

A theatre director ensures every paying audience member can see the stage and hear the dialogue — the cheap seat is still a designed seat. A sports arena makes no such guarantee: the ticket grants admittance, and the experience is whatever happens. Both are legitimate. The difference is the scope of the obligation. The template economy has been the arena — every user admitted, presence guaranteed, experience variable, entirely dependent on which template happened to be chosen.

**Why it can't come from a prompt:** the correct design unit is context, not pixels. A pixel is a rendering instruction, not a design decision — its meaning changes with every hardware generation, which means designing in pixels means designing for today's constraint, one that expires with the next device release. A governing ratio — the column unit, the space token, the type scale — is a first-principles decision a document makes once; a prompt can only ever ask for an approximation of whatever the model has seen before.

**Concrete example:** the iPhone 1 was 320 pixels wide; the iPhone 15 Pro is 1179. The phone is roughly the same size in the hand. The pixel count tripled; the hand, the reading distance, and the attention span did not change. A screen governed by context — handheld/close/one-hand, seated/medium/two-hands, ambient/long-distance/passive — survives that tripling without being redesigned. A screen governed by pixel count does not.

---

## Context

*Adapted from Design for the AI Era: Paradigm Shift — Context chapter.*

**What it governs:** not where the user is, but the path they took to get there — the journey, replacing the page as the unit of design.

The web took a preproduction artifact and shipped it: the wireframe became the page, the storyboard became the experience itself, and the edit — the governed transition between states — was never made. Comics solved this differently: the panel is authored, but the gutter between panels is where the story actually happens, and the artist governs that space as deliberately as the panel itself. The page, by contrast, is an address. It says where something is. It says nothing about who arrived, what brought them, or what they were doing before they got there.

**Why it can't come from a prompt:** context is directional, and direction is a decision, not an inference. A Visitor moving toward Researcher carries curiosity into depth. A Researcher moving toward Visitor carries authority into encounter. Same edge, opposite intent, different governing decisions — a distinction a prompt has no mechanism for holding, because a prompt answers one query at a time with no memory of the path that produced it.

**Concrete example:** the state stack. A user moving from a deep media state back toward research doesn't reset — the system releases what was left behind, visually, as media assets fade rather than vanish. A user deepening carries their path forward as reduced-opacity context: present, foundational, not dominant. No third-party cookies, no behavioural surveillance — the system knows what happened *within itself*, not who the user is across the internet.

---

## Content

*Adapted from Design for the AI Era: Paradigm Shift — Content chapter.*

**What it governs:** what fills the governed context — not a single, approved, context-agnostic version of a piece, but a source record with a design document holding the selection rules for each state.

Content in the digital era suffered an approval collapse: because content is approved once, it must be context-agnostic by design, flattened so it can sit anywhere. The content that reaches a casual visitor becomes identical to the content served to a researcher. AI trained on the aggregate output of that collapse inherited the same flattening — different prompt, same surface.

**Why it can't come from a prompt:** the alternative is atomic content, governed by a document, not regenerated per request. One source record, one design document holding the rules for each context state — the content does not multiply, the governing decisions do the work. A prompt regenerates from scratch every time; a governed selector reveals the correct pre-authored assembly.

**Concrete example:** a single Vermeer painting, three encounters. A Visitor gets a headline — *"Light that has lasted four hundred years"* — narrative, short paragraphs, no footnotes. A Researcher gets full attribution, citation, provenance, no truncation. A Media enthusiast gets the film review, the credits, the interviews. The object doesn't change. The persona governs the structure, the weight, and the presentation, and the design document holds the selector that decides which one a given person receives.

---

## Time

*Adapted from Design for the AI Era: Paradigm Shift — Time chapter.*

**What it governs:** memory as a structural coordinate, not an afterthought — what a system holds, what it releases, and what that says to the person it's holding it for.

Experience and time are not merely related; they are the same thing. Remove time and there is no experience left, only simultaneity, which is noise. The stateless screen resets to zero on every visit — not because time was unimportant, but because memory was never designed in. Every reset discards a relationship: a system that resets to zero tells the user *we do not know you, start again* — a structural message, not a neutral default.

**Why it can't come from a prompt:** decay rules are deliberate, human decisions with ethical and experiential implications — how long a system remembers, what it forgets, what it holds even after a person has moved on. A prompt has no persistent state to make that decision about; every prompt is, definitionally, a reset.

**Concrete example:** the state stack's motion grammar. Deepening gets a dissolve — the past carried forward, visible at reduced opacity, present but not dominant. Pivoting gets a cut — the previous moment closed cleanly, the direction change acknowledged. The decay rules are authored once, in the design document, before any user arrives; the execution — different for every unique state stack — cannot be done by hand, but the rule that governs it was never automatic to begin with.

---

## Trust

*Adapted from Design for the AI Era: Paradigm Shift — Trust chapter.*

**What it governs:** accountability — who is responsible for what a system does, and how anyone would know if something went wrong.

Trust is a relationship with two distinct sides. The creator's obligation is to govern: to name the rules, make them auditable, and stand behind them. The user's obligation is nothing — trust from the user is a gift extended solely on evidence, and when evidence is absent and decisions are untraced, that gift is withheld. The screen's history, largely, has been trust without accountability: decisions made, nothing named, nothing auditable, no one able to say afterward why the system did what it did.

**Why it can't come from a prompt:** a prompt produces an output, not a rule. There is nothing in a single generated response to audit against, because there was no prior, named commitment the response can be checked against. A design document's rules are the opposite: written down before the build, testable at any point, standing even after the person who wrote them has left the project.

**Concrete example:** every decision in the design document — persona, context states, content rules, time rules — has a named place, a trigger, a result, and an author. Readable by the designer, the client, the developer. Auditable at every point. The design document is the discipline's answer to a literacy gap the printing press took centuries to close for readers, and that AI-generated interfaces currently have no equivalent for at all.

---

*Persona is the governing input across all five. See `/polygon-grammar` for how persona itself is structured, and `/governance` for how a real person's position is sensed at request time.*
