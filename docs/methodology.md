Title: The design document is the product. The screens are the consequence.

*Title line from Design for the AI Era: Paradigm Shift. This essay is original argument, not adapted from the book.*

---

The design document is the product. The screens are the consequence.

That line sounds like a slogan until you sit with it. So sit with it for a moment before the argument starts.

## The bible and the episode

A long-running procedural show survives writer turnover that would sink almost any other kind of production. Different scripts every week, different guest directors, sometimes an entirely different writers' room by season four — and yet the show stays recognisably itself. The detective still questions suspects the same way. The station still feels like the same station. The tone never drifts far enough that a viewer notices the seams.

What holds it together is not any individual episode. It is the bible — the internal document that defines who these characters are, what the show believes, what it will and will not do, written once and consulted constantly. A new writer does not reinvent the show from a blank page. They read the bible, and the bible tells them what an episode of this show is allowed to be.

The episode is downstream of the bible. It is the consequence of a decision made earlier, elsewhere, by someone whose job was to define the show rather than write any single instalment of it.

A governed design document works the same way. It is authored once, by someone whose job is to decide what a product should be and for whom. Everything generated afterwards — every screen, every layout, every piece of interface a user actually touches — is an episode. The document governs. The screen is the consequence.

## What this is not

Two terms have entered the AI-and-design conversation recently that sound, on the surface, like they might be describing the same thing. They are not, and the difference is worth being precise about, because the precision is the whole argument.

DESIGN.md is a format for specifying design tokens and visual identity — colours, spacing, type — written so that a tool such as Stitch can consume it directly. It is genuinely useful for what it does. It is not a governance layer. It has no concept of a persona, no model of who is reading or using the product, no mechanism for producing different, equally correct experiences for different people from the same source. It specifies values. It does not specify intent.

constitution.md, from the spec-driven development world, does something adjacent but unrelated: it specifies immutable principles for how code gets written — testing discipline, architectural rules, the non-negotiables a coding agent must respect. It has nothing to say about design at all.

Neither of these is a competitor to a design document in the sense this essay means. They are details — the kind of thing a full design document specifies and then generates, the way a show bible might specify a recurring set's colour palette without that palette being the bible itself. A token file answers "what are the values." A code constitution answers "what are the rules for the code." Neither answers the only question that actually matters first: what should this be, and for whom.

That question is what a design document, properly understood, is for.

This document has a name: **EXPERIENCE.md.** Wherever this essay says "the design document," it means that artifact — specifically, not generically. It is where the persona grammar, the five dimensions, and the rules that govern both actually live.

## One document, many generations

Here is where the mechanism gets specific, and where it stops being metaphor.

**The design document is the single input.** Not one document per user, not one per screen — one document, governing everything that follows.

**A polygon grammar defines who someone can be, inside that document.** Not a fixed audience, not a single imagined average reader, but a structured space of possible states — named positions a real person can occupy, with the relationships between those positions specified explicitly enough that moving from one to another is a defined transition, not a guess. This is the vocabulary the document uses to describe *who*, before anything about *what* gets decided.

**A sensing layer places a real person inside that vocabulary.** Not a login, not a tracked profile sold to advertisers — a local read of intent, depth, and history, computed on the reader's own device and never transmitted anywhere. This is what tells the system where, right now, a specific person actually sits in the space the document defined.

**The document is then refracted through that position, not regenerated for it.** One source, one angle of incidence, one specific output — the way white light through a prism becomes a particular colour depending on the angle, without the light itself needing to change. Multiple people encountering the same document produce multiple different, equally legitimate outputs. None of them is a compromise. None of them is a guess standing in for the others.

**Five dimensions are what actually gets configured in that refraction.** Screen, Context, Content, Time, and Trust are not a checklist applied afterwards — they are the axes along which the one document becomes a specific, particular screen for a specific, particular person.

The chain, in full: the document authors the grammar. The grammar defines the space of who someone can be. The sensing layer finds where a real person sits in that space. The refraction produces an output governed by that position, along five defined dimensions. The screen is what comes out the other end.

## What this looks like from four different chairs

The clearest way to see this is not through the mechanism itself but through who it actually changes things for. Four people touch the same governed piece of work, and the document changes what each of them experiences.

| Who | Before a governing document | After one |
|---|---|---|
| **The designer** | Builds against an abstract "user" — a composite nobody actually is — and guesses at how to serve every audience from one compromised layout. | Designs against named, defined states. A choice can be defended against a specific model instead of a hunch. |
| **The author** | Imagines one reader while writing, usually themselves a few years younger, with no way to know who the piece actually reached. | Writes toward a governing line stated before the draft is even finished — and knows, afterwards, which real, named audiences the piece actually served. |
| **The publisher** | Holds editorial identity in a mission statement nobody can audit against actual decisions. | Accumulates a queryable record of what was actually stood for, piece by piece, not aspirationally. |
| **The reader** | Gets the same experience as everyone else, regardless of who they are or what they already know. | Gets an experience calibrated to where they actually are — not simplified, not elevated, precisely theirs. |

Take the reader's chair a moment longer, because it is the one furthest from where any of this work happens and the one where the effect is easiest to feel.

Julian clicks a link a colleague sent him. Two paragraphs in, he is still reading — unusual, because most things he clicks on lose him by now. What is holding him is not an algorithm noticing a shared keyword. It is a governing line, written by the author before the draft was finished, naming why this piece exists and what it assumes he brings to it. He never sees that line. He never needs to. It reaches him anyway, in the fact that the piece he gets next continues his actual question instead of guessing at a topic.

On his second visit, the layout looks different — not broken, recalibrated. Denser where he had shown depth, lighter where he had not. Nothing about this required him to log in, declare a preference, or be tracked across the web. The signal that placed him where he was lived in his own browser the entire time, and travelled with him precisely because it was never anyone else's to hold.

Neither of those experiences was generated by a prompt someone typed while looking at Julian's screen. Both were the consequence of a document, authored once, upstream, doing exactly what it was built to do.

## Where AI actually sits

None of this is an argument against AI having a real role in design work. It is an argument that the role is narrower than most of the current conversation assumes, and that it sits in exactly one place: upstream, in authoring.

In **decisions**, AI may assist the person authoring EXPERIENCE.md and the content it governs. It can test a persona grammar against edge cases, surface options the author had not considered, draft candidate language for review. But the decision of what the document actually says — what a piece is for, who it assumes its reader to be, what a product should become — stays with the author. AI can widen the set of things being considered. It does not get to choose which one governs. Everything it produces here is reviewed and approved before it becomes part of the governed record.

At the moment a real person actually arrives — the moment a screen gets shown — there is no AI in the room. Prism does not generate a response. It reveals one: a treatment that was already authored, already reviewed, already governed, selected because the sensed context matches a position EXPERIENCE.md already defined. This is mechanical, not generative. A prism does not create the wavelength it makes visible. Prism does not create the screen it makes visible either.

Most of what currently gets called "AI-assisted design" collapses authoring and delivery into a single step: a prompt that decides and produces in the same instant, with no document behind it, no review between the decision and its execution, and no way to audit afterward why a person saw what they saw. That collapse is not a shortcut. It is the actual failure mode — the reason generated interfaces so often feel like an average of everything that came before them, answerable to nothing in particular because nothing in particular governed them.

EXPERIENCE.md refuses that collapse. It is the reason authoring and delivery are two separate acts, done at two separate times, by two different kinds of agency — one of them human and reviewed, the other mechanical and auditable.

## The screens are the consequence

Return to the line the essay opened with, because by now it means something more specific than it did at the start.

The design document is the product — not metaphorically, as a way of saying design matters, but literally, as the description of what the actual work is. The document is where the governing decisions live: who a person might be, what a piece is for, what a product should become and for whom.

The screens are the consequence — not metaphorically either. They are the literal output of a pipeline that starts with EXPERIENCE.md, passes through a grammar of persona, senses a real person's position inside that grammar, and reveals — not generates — the treatment already governed for that position along five defined dimensions. Every screen a person actually touches is downstream of a decision someone made before any screen existed.

The bible governs. The episode is what airs. Everything else is production.
