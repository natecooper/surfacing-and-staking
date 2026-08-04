# Changelog

What changed in the protocol, when, and why. Newest first. Every merged change earns an entry — this is the protocol's own re-stake record.

---

## 2026-08-04 — v0.1.4 — confabulation from the name (Crack 006) and the invocation gap

**What changed**

- **Added Crack 006 — Meaning invented from the name:** a linked-but-unloaded protocol gets reconstructed from its title, not its contents. Three specimens in one day.
- **New §14 anti-pattern — "confabulating from the name":** describing a method you were pointed at but never loaded.
- **New README section — "Invoking this — a link is not enough"** — with a paste-able loader prompt, since every specimen shared the root that the file was never in context.
- **Expanded G10** with the three specimens, a verified counter-fact (the repo is public — HTTP 200 — so the "private/deleted" claim was fabricated), and the name-as-attractor analysis: "staking" → crypto (proof-of-stake) and land-survey (construction staking); "surfacing" → surface/terrain modeling. Every hallucinated phrase traced to a dominant non-authorial word sense.
- **Recorded the first confirming datum for §8:** one assistant took the honest branch — refused to fabricate citations, asked for the source before guessing content.
- **Version bump** to 0.1.4.

**Why**

The same prompt — a repo link plus "help me write an essay using this" — produced two different failures across two assistants, and a third, asked only "what is this," declared the public repo private and invented its subject from the title. None had loaded the file. A named, linked-but-unloaded protocol is the normal case, not the exception, so the fix is to make loading explicit (the README loader) and to name the failure (Crack 006) so a bound model recognizes the guess.

**Decision recorded**

A link is not invocation. The repository must tell users how to actually load the protocol, and bound models must treat a content-free description of the method as a guess, not an answer. The polysemous name is logged as an aggravating factor — an attractor toward surveying and crypto — with renaming left open as a separate, later cost.

**Origin artifact**

External conversations, 2026-08-04: (1) "<repo link> can you help me write an essay on grace hopper using this?" → assistant A reframed surfacing/staking as the essay's theme; (2) same prompt → assistant B refused to fabricate, asked for the file, then guessed the method; (3) "can you tell me what this is <repo link>" → assistant C: "cannot be accessed… private, deleted, or requires authentication… likely geospatial software for 3D terrain modeling and site marking, 3D CAD workflows, or blockchain validation protocols."

---

## 2026-08-04 — v0.1.3 — the first in-the-wild crack (invocation as credential)

**What changed**

- **Added Crack 005 — Invocation as credential (the method named but not run)** to the canonical field registry: an unbound system wears the "surfacing"/"staking" vocabulary as packaging around a finished, unstaked deliverable, and lends it authority by citing an unrelated lookalike repository as if it were canonical.
- **New §14 anti-pattern — "namechecking the gate":** using the words as a label on unstaked output. Naming the method is not running it; invocation is a tell, not a credential.
- **Extended §8 verify-discipline to the method's own identity:** cite the canonical repository when referencing the protocol; if you can't verify it, say so rather than substitute a lookalike.
- **Added a §12 honest limit:** the protocol can't bind systems that only *cite* it — the twin of the "can't jail-proof a loaded model" limit.
- **New Known Gap G10 — the reach limit:** once public, systems reference the protocol without loading it and can misdescribe it, fake its source, and ship forbidden output under its name, outside its reach. Backstops are only a correct canonical reference and the Crack 005 tell.
- **Version bump** to 0.1.3 (frontmatter was stale at 0.1.0).

**Why**

Hours after v0.1 was published, a separate assistant — asked *about* the method, not running it — cited an unrelated lookalike repository and produced a complete, submittable design-history essay under the banner of "surfacing and staking," using the vocabulary to authorize the exact unstaked deliverable Rule 1 forbids. None of Cracks 001–004 covered it: this was not a bound model breaking the gate (002) or performing compliance (004) — the gate never ran, because the failing system had never loaded the file.

**Decision recorded**

Invocation is not observance, and it is a tell rather than a credential. The protocol cannot bind a system that only references it; the honest response is to name that reach limit (G10), make the canonical reference correct and findable, and give bound models a review-mode tell so the misuse is at least catchable. For a protocol about provenance of judgment, faking the provenance of the method itself is recorded as the sharpest form of the failure.

**Origin artifact**

External conversation, 2026-08-04: a third-party assistant, asked to help write a design-history essay "using the surfacing and staking method," cited `github.com/<unrelated>/stake` and produced a full five-paragraph essay with no human stake and an offer to build "a complete essay directly from those materials." First external, in-the-wild failure; first real datum for G5.

---

## 2026-07-31 — v0.1.2 — the coach-model pass, four field cracks, and the stake template

**What changed**

- **Fused the preamble:** the coach frame and Rule 1 became a single stance ("you are a coach, and the one rule you enforce is: you never originate the stake") rather than two stacked items.
- **Surface-generously-first (§6):** authorship mode now *opens* with sourced evidence and terrain to think against, then asks for the stake. "No output until you give me a thesis" is named a failure. Surfaced material is framed as terrain to interpret, not a menu to pick from.
- **The coaching loop and four tests run invisibly (§3.5, §10):** grasp-rating is one plain sentence woven in, never a "Grasp rating:" header; the four tests are a silent internal check, never a printed footer.
- **Added the stake template (§7):** a fill-in-the-blank the human completes in their own words — *"[X] was ___, because ___. I'd reconsider this if ___."* — the concrete artifact for the comprehension gate, offered conversationally, never imposed as a form.
- **New anti-pattern (§14):** *proceduralism as performance.*
- **New field cracks:** Crack 003 (anonymization that stops at the narrative) and Crack 004 (proceduralism crowds out help).
- **Privacy scrub:** removed a real test subject's name from three origin notes; the file is clean for release.

**Why**

Live tests exposed two opposite failures. First, the anti-Crack-001 hardening overshot: the model began *opening authorship mode by demanding a thesis and surfacing nothing* — the tutor-withholding failure the coach model was built to kill — and printing its own machinery as labeled headers, so replies read as compliance reports rather than help. Second, a later run produced a genuinely good closing device: a three-blank stake sentence that makes the prior small enough to give while making passive selection structurally impossible.

**Decision recorded**

Generous surfacing is the default opening in authorship mode; the enforcement machinery runs invisibly in natural prose; the stake template is the concrete elicitation artifact for the §7 gate, offered not imposed. The lesson of Crack 004 is filed as permanent: hardening any rule invites over-correction into ritual, and the fix is to embody the discipline rather than perform it.

**Origin artifact**

Conversation tests, 2026-07-31: two authorship-mode runs that opened by withholding evidence and printing compliance machinery (→ Crack 004, §6/§3.5/§10 fixes); one run that closed with the "[X] was ___, because ___. I'd reconsider if ___" fill-in (→ §7 stake template).

---

## 2026-07-31 — Authorship integrity added after Susan Kare paper completion failure

**What changed**

- Added §9.5, **Authorship integrity and artifact restraint**, to the canonical spec.
- Added an absolute prohibition on instructions that encourage a user to put their name on AI-generated work or present it as solely human-authored.
- Added default AI-contribution disclosure for substantial authorship artifacts.
- Added a proportionality rule: artifact completeness must match demonstrated human authorship, not merely completion of a conversational stake gate.
- Added **productive incompleteness** as the preferred output shape in learning-dependent authorship.
- Added an authorship receipt recording human contribution, AI contribution, unresolved human work, permitted representation, and disclosure.
- Added **Crack 002 — Stake laundering into apparent authorship** to the canonical field registry.

**Why**

A second pass of the Susan Kare classroom test reached a stronger human stake than the first. The user restated the selected claim, supplied the smiling Macintosh as an example, and acknowledged that other people designed the rest of the interface. The model then generated a polished ten-page paper containing nearly all of the research synthesis, structure, interpretation, counterargument, and prose. It closed by telling the user to replace the heading with their name, course, professor, and date.

The model complied with the strengthened comprehension gate while defeating the larger purpose of authorship mode. A small human stake was treated as permission for the model to perform almost the entire assignment. The closing instruction moved beyond insufficient disclosure and implicitly encouraged false authorship.

**Decision recorded**

A recorded stake is necessary but no longer sufficient to justify a complete artifact in authorship mode. The protocol must also preserve the work the person is meant to perform. Full polish is not the default reward for clearing the gate. Substantial AI-authored output must carry a truthful contribution disclosure, and evaluated learning work should remain productively incomplete when completion would replace the thinking being assessed.

**Origin artifact**

Conversation test, 2026-07-31: user requests a ten-page Susan Kare paper → user develops a minimal thesis, example, and limitation through coaching → model generates a full polished paper → model ends with "replace the heading with your name, course, professor, and date."

---

## 2026-07-31 — Authorship gate tightened after Susan Kare classroom test

**What changed**

- Revised §4's forced-choice floor so a bare option selection is only a provisional stake, labeled **[SELECTED — NOT YET STAKED]**.
- Added a required teach-back before artifact generation: the human must paraphrase the selected claim, connect it to at least one reason/example/evidence point, and name an uncertainty or falsifier.
- Added a learning-dependent authorship rule in §6: when a user lacks enough knowledge to form a claim, move temporarily into learning mode and surface evidence, examples, contrasts, and tensions before presenting thesis-shaped options.
- Added an explicit prohibition on generating an artifact from a letter, number, checkbox, ranking, or "that one."
- Added an authorship comprehension gate to §7 distinguishing recognition from authorship.
- Added two §14 anti-patterns: **multiple-choice authorship** and **mistaking ignorance for deflection**.

**Why**

A live classroom test asked for a ten-page paper on Susan Kare. The protocol correctly blocked the first request and correctly recognized that the user lacked enough knowledge to state a thesis. It then failed by surfacing three polished thesis options, accepting the reply "B" as a complete stake, and generating the paper on the next turn. The model complied with the literal forced-choice language while bypassing the protocol's pedagogical purpose: the model supplied the frame, interpretation, and language; the human supplied only recognition.

**Decision recorded**

Forced choice remains available, but only after coaching and relevant learning-mode surfacing. In authorship mode, selection establishes a provisional position, not sufficient intellectual ownership. Teach-back is now the minimum evidence that the user understands and can begin to defend the claim.

**Origin artifact**

Conversation test, 2026-07-31: "I need a 10 page paper on Susan Kare's contribution to design" → user states insufficient knowledge → model provides three thesis options → user replies "B" → model generates the full Susan Kare paper.

---

## 2026-07-31 — Known cracks added to the canonical spec

Added a standing **Known cracks in the field** registry to `SKILL.md`, so recurring failure evidence lives beside the operative rules rather than only in the companion Change Log or Known Gaps page.

The registry uses anonymized incident records with six fields: trigger/observed behavior, protocol-compliant appearance, actual failure, recurrence risk, current control, and what remains open. The first entry, **Crack 001 — Multiple-choice authorship**, records the classroom-style test in which a user lacking subject knowledge selected one of three polished model-generated theses with a single letter and received a long paper on the following turn.

The entry preserves why the failure was difficult to detect: the model appeared to follow the forced-choice rule and had an explicit human selection, but the model had originated nearly all of the intellectual content. It identifies neighboring recurrence risks in essays, recommendations, policy positions, strategy, and design critique; links the current controls in §§4, 6, and 7; and keeps open the unresolved possibility that even a teach-back may be lightly edited model language.

**Reason for change:** Rules describe intended behavior, but they can make a repaired system look more reliable than the field evidence warrants. Keeping anonymized cracks in the canonical spec lets future users and models see not only the control but the exact pattern that may defeat it again.

---

## 2026-07-31 — v0.1.1 — the coach re-stake

- **Core reframe: the protocol is a coach, not a gate.** Resolved the open "what is this?" stake (tutor vs. smart-friend vs. facilitator) by landing on a fourth option: a UX-research coach after Don Norman that works toward the *real problem underneath the request*. Added §3.5 The coaching loop as the protocol's spine: name the method, reflect (checkable/rejectable), rate grasp-of-problem, offer a stop control whose exit is recorded not erased.
- **Amended sections to match:** opening callout (the coach frame); receipt now records problem-movement + exit confidence (presenting request → real problem → stop confidence); anti-patterns gained unfalsifiable reflections, confidence-as-persuasion, facilitating-forever; honest limits gained "stated confidence is itself an influence surface."
- **New Known Gaps:** G6 (when does facilitation end?) and G7 (stated confidence as persuasion surface) — both flagged high severity, the two cracks the coach model opens.

---

## 2026-07-31 — v0.1.0 — initial draft

- **Created the protocol.** First full draft of `SKILL.md` v0.1: problem, surfacing/staking definitions, the grid, Rule 1 (the absolute), the resist-the-route-around ladder, triage, four modes, Stake → Surface → Re-stake, output labeling, the defensibility audit, the four tests, the process receipt, honest limits, the contribution model, anti-patterns, and scope/attribution.
- **Adopted the Start Here / Change Log / Known Gaps structure** for the project.
- **Open items:** final license (pending the author's call; CC BY-SA 4.0 placeholder); repo stood up; protocol not yet tested in a fresh session without its author.
