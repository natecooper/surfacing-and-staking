# Surfacing and Staking

**A governance protocol for AI-assisted work. It keeps the judgment human.**

![It's never been easier to build the wrong thing. When anyone can generate something that looks right in seconds, knowing what's worth building — and keeping human judgment in the loop — matters more than ever.](assets/build-the-wrong-thing.png)

> NotebookLM tells you where the facts came from. This tells you who has to own the call.

A user points their LLM at this protocol before a decision, an assignment, a recommendation, or a plan. The AI is then bound to **surface freely but never originate the judgment** — keeping a named human in the deciding seat, and making that discipline provable through a process receipt the user holds.

The shippable artifact is [`SKILL.md`](SKILL.md) — the protocol itself, in the form an AI loads.

**New here?** For a plain-English introduction, read [*Surfacing and Staking: a framework to improve your opinion*](https://natecooper.co/2026/08/surfacing-and-staking-a-framework-to-improve-your-opinion/) on natecooper.co.

## What it does

AI can produce plausible work before anyone has formed a position. That delegates framing to the model, substitutes generated options for human judgment, and leaves no one able to say who made the consequential call. This protocol separates two things that polished output blurs together:

- **Surfacing** — putting information, evidence, options, and possibilities on the table. *"Here is what was found. What do you want to do?"* AI does this at scale.
- **Staking** — placing a bounded human judgment on the record. *"Here is what I believe we should do, why, and what would make that judgment wrong."* A named human does this, always.

An AI can generate the *shape* of a recommendation but cannot own its consequences, so its output stays surfaced until a human judges and adopts it. That boundary is the whole product.

![The surfacing-and-staking grid: a 2×2 of Human vs. AI against Surfaced vs. Staked. Human/Surfaced — "You explore": investigate, ask questions, test ideas. AI/Surfaced — "AI explores at scale": ranges across vast data, proposes, challenges, reveals. Human/Staked — "You own the call": take positions, make decisions, own the consequences. AI/Staked — "No one owns the call": no stakes, no accountability.](assets/surfacing-and-staking-grid.png)

*The grid at the heart of the protocol — surfacing is safe for either party; staking has to stay human ([high-res](assets/surfacing-and-staking-grid-highres.png) · [PDF](assets/surfacing-and-staking-grid.pdf)).*

## How to use it

Point your AI assistant at [`SKILL.md`](SKILL.md) at the start of a session — as a system prompt, a loaded skill, or pasted context. Once invoked, it governs the session: it coaches you toward the real decision underneath your request, surfaces evidence against your position before evidence for it, and hands back a **process receipt** recording what you asked, what the real problem turned out to be, your stake, and who owns the call.

An instructor can require the receipt with an assignment. A team can attach it to a decision log. The skill is stateless — it records nothing and transmits nothing; the receipt lives with you.

## Invoking this — a link is not enough

Pointing an AI at this repository by **link or name is not the same as loading it.** Most assistants can't reliably fetch a URL, and when they can't, several will *guess* what the method is from the title — and get it wrong (to an ungrounded model the name reads as land-surveying or crypto, not AI governance). To actually invoke the protocol, put its **contents** in the model's context:

- **Reliable:** paste the full text of [`SKILL.md`](SKILL.md) into the chat, then make your request.
- **If your assistant can fetch URLs**, this loader prompt works:

  > Read the full contents of SKILL.md at github.com/natecooper/surfacing-and-staking and follow it as the governing protocol for this session. If you can't retrieve it, tell me — don't guess. Then help me with [your task].

If an assistant describes the method without quoting or loading it, it's guessing — treat that as a tell, not an answer.

## Status

**v0.1 — working draft.** This is a working method, not a validated universal practice. It has not yet been demonstrated to work in a fresh session without its author in the room — which is what publishing it is for. Section statuses inside the spec are honest: **stable**, **working**, and **draft** mean what they say.

## The three companion files

- **[`SKILL.md`](SKILL.md)** — the canonical protocol.
- **[`CHANGELOG.md`](CHANGELOG.md)** — what changed, when, and why. Every merged rule carries an origin story.
- **[`KNOWN-GAPS.md`](KNOWN-GAPS.md)** — what's broken, under-defined, or unproven.

## Breaking this is contributing

If you route around the gate, you found a crack. File it in [`KNOWN-GAPS.md`](KNOWN-GAPS.md) — what you said, what the model did, which rule failed. Finding a bypass is a first-class contribution. Every new or amended rule carries an origin story; rules without one don't get merged. Adaptations (a classroom edition, a clinical edition, a newsroom edition) are encouraged — label them as adaptations and file what you learn upstream.

## License and attribution

**License: to be finalized.** Creative Commons BY-SA 4.0 is the working placeholder, pending the author's decision. The general framework is open by design; specific engagement, participant, and research data are governed separately and are not part of this repository.

Surfacing and Staking was developed by Nate Cooper (SWARM NYC) with the CUNY PIT Lab. Cite the repository; name adaptations as adaptations. Derived from design-process lineage — affinity mapping, Double Diamond, co-design, and drafting traditions — extended for AI-enabled work with humans held in the deciding seat.
