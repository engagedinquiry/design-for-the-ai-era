# /prism — the reveal/split mechanism

*Register: Technical, following from `/dimensions`. First full formal statement of the mechanism.*

*Adapted from Design for the AI Era: Paradigm Shift — Prism chapter.*

---

## A prism does not create light

A prism does not create light. It reveals what light contains.

Raw light — white, undifferentiated — enters the glass. The prism's geometry separates it into constituent wavelengths. Each wavelength emerges at a different angle. The spectrum is not added by the prism. It was always in the light. The prism makes it visible, and makes a specific colour available to whoever is positioned to receive it.

This is what happens to content in Prism. Content arrives from a data store as raw material — undifferentiated, without rendering instructions, already authored and already governed by the design document. Prism separates it according to who is receiving it: their intent, their context, their position in the experience. A specific experience emerges. **Not because Prism added something to the content, but because it reveals what the content already was for this user at this moment.**

Prism does not generate. It splits.

## Not a browser

In a Browser model, the server decides what experience the user receives, encodes that decision in HTML, and transmits it. The browser app executes the decision. The user receives what the server chose to send.

In Prism, the app on the device decides. The server supplies content, assets, addresses. Prism reveals which governed treatment applies, using context it holds locally — the user's intent, their journey, their persona position at this moment. The server does not need to describe what experience Prism will produce. The governance is not the server's job — it was already done, upstream, in the design document.

| | Browser | Prism |
|---|---|---|
| Who governs the render | The server | The design document |
| Where the user's context lives | The server | The device |
| What the response contains | A page | Content, without rendering instructions |
| How the experience is produced | What the server chose to send | What was already true, revealed for this position |

## The spectrum

Every Prism-governed app can produce a spectrum of experiences from the same content. At one end, a user in one context receives content presented one way. At the other end, a user in a different context receives the same content presented differently. Between the ends, every position produces a governed rendering specific to the context that produced it.

The spectrum is authored, not generated at request time. A designer defines the positions — the personas, the treatments, the hierarchy appropriate to each — in the design document, before any request arrives. The designer does not define every point on the spectrum; they define the vertices and rules for the points between them. **Prism reveals the point that was already implied.**

White light contains all wavelengths. The prism reveals the one that corresponds to the angle of incidence. Prism the app holds all governed treatments. The user's context state is the angle. The experience that emerges is the colour — specific, already governed, revealed rather than produced.

## How this works

```
query (content, assets, URLs)  →  Prism  →  runs on rules
                                       ↑
                          intent + context state
                            (sensed locally — see /governance)
                                       ↓
                                  response
```

Intent and context state are supplied by a local sensing mechanism — how that mechanism is implemented is a governance question, not a Prism question. See `/governance` for what a governed system requires of it.

## What the user experiences

A user in Prism does not navigate to pages. They express intent — through search, selection, or behavioural signal. Prism queries the data store, receives already-governed content, and reveals the treatment appropriate to the user's current context.

**Immediately legible:** the experience responds to who the user is, not just what they asked for. The same query from a user early in their journey produces a different experience than the same query from a user who has spent time with the product. The content may be the same. The rendering — hierarchy, prominence, framing — reflects where the user is.

**Not immediately legible:** the user's data never left the device. No server received their behavioural history. No platform logged their journey. The experience is calibrated because the sensing is local and the treatment was already governed — not because a model is deciding what to show them in the moment.

## Discovery remains

Prism does not replace the web as a discovery surface. A user finds a product or a company through search, through a link, through a public presence. The front door is still the web. This does not change.

What changes is the threshold. In a browser, crossing the threshold means entering a server-controlled experience. With Prism, the threshold is where the browser's authority ends. The user discovers through the web and enters through Prism. From that point, the treatment they receive was already decided — Prism only reveals which one.

**The two paradigms coexist: the web for finding, Prism for revealing.**

---

*See `/governance` for the sensing mechanism Prism depends on, and `/dimensions` for what the design document governs before Prism ever runs.*
