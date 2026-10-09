# Changelog

What changed in the protocol, when, and why. Newest first. Every merged change earns an entry — this is the protocol's own re-stake record.

---

## 2026-10-09 · v0.1.7 · README repositioned for the champion reader

**What changed**

- **New tagline:** "AI made polished output cheap, and polish reads as judgment. This keeps the judgment yours, and helps you prove it." It replaces "a sparring partner for thinking with AI."
- **Built-for line** directly under the tagline, naming the reader: the person inside an organization who has to take a project to the people whose yes they need.
- **New section, "Steelman your stakeholders":** before you take a stake to the people whose yes you need, surface each one's strongest objection and re-stake, and a re-stake can be a smaller project, a different one, or none. It is worded as an instruction to the reader, because `SKILL.md` §7 Phase 2 surfaces the case against a stake but does not reliably name and voice each stakeholder. It points to §11 for roles rather than restating them.
- **Second sample receipt, the champion case:** a fictional proposal for a policy-docs assistant, authored here, using the §11 roles (author, judge, consumer, consequence holder) because more than one person holds the call.
- **"Who it's for"** leads with a champion row and carries a note that stakeholders show up as the case you surface: they may read your receipt, and they never run the tool to judge your work. The line ranking education as the sharpest first fit is removed; where the method has been used belongs in Status, stated as fact.
- **IT pointer and internal-copy note:** a line under the opener sends IT and security reviewers to their section, which now sits in a GitHub note box and adds that editing your own copy for internal use creates no obligation to publish it.
- **Receipt described as evidence, not proof,** to match `KNOWN-GAPS.md` G4.
- **Section order:** How it works (renamed from "What it does"), Who it's for, Steelman your stakeholders, For IT / security review, How to use it, Where this sits, then the rest unchanged.
- **Version bump** to 0.1.7.

**Why**

The recurring critique of the README was that it named no persona and no core problem. The method was built for one reader in particular: a person inside an organization championing a project, who has to get it past IT, leadership, the people whose work it changes, and anyone else whose yes it needs. The README opened as a general sparring partner and led its audience table with education, so neither the opener nor the table said who it was for. Stakeholders are framed as the people who hold a constraint the project has to fit, never as opponents, because the README travels by being forwarded to exactly those people.

**Decision recorded**

The README leads with the champion reader and the steelman-your-stakeholders case. Stakeholders appear as the objection being surfaced and may read a receipt; they are never users who run the tool to judge someone else's work. The README promises only behavior the protocol has: naming and voicing each stakeholder stays a reader instruction until a protocol-side rule earns an origin story of its own.

**Still pending**

License and attribution are unchanged in this release. The license is still marked to be finalized, and the attribution line is unchanged; both wait on the author's decision. Status keeps its "not yet demonstrated without its author in the room" sentence until there is evidence to change it.

**Origin artifact**

Positioning call, 2026-10-07, and the internal handoff spec that followed it: an analysis of who the method was built for, written in answer to the recurring "who is it for" critique. Rebuilt on top of v0.1.6 after an earlier local working copy of the same changes was lost before it was pushed.

---

## 2026-08-17 — v0.1.6 — progressive disclosure: routing table, reference split, and a 27% context cut

**What changed**

- **New §0 Routing** at the top of `SKILL.md`: a symptom-to-section table — the request in front of you on the left, the sections to run on the right — plus a note on which reference files exist and are deliberately *not* loaded yet. A model that only previews the head of the file now lands the whole dispatcher.
- **Known cracks 001–006 moved to `references/cracks.md`**, loaded on demand. §13 keeps the pointer and the reason the registry exists; §14 keeps the operative rule from each crack and states that the `Crack 00N` pointers resolve to that file. The rule is enough to comply; the crack explains why the rule may still fail.
- **Two §12 limits moved to `references/limits.md`** — that the protocol can't bind systems which only cite it, and that a receipt can be fabricated. Both describe where the protocol's reach ends rather than how to behave inside an invoked session. The four limits that govern in-session conduct stayed.
- **Contribution mechanics moved to a new `CONTRIBUTING.md`** — rule format, anonymization scope, adaptations, section-status discipline. `SKILL.md` §13 keeps only what a model acts on mid-session: report which rule broke, and where to file it.
- **Four dated origin notes removed** from §4, §6, and §7, each already recorded in fuller detail in this changelog. Two undated design rationales were kept, since nothing else records them.
- **`metadata.version` is now a quoted string** (`"0.1.6"`). The Agent Skills spec defines `metadata` as a map of string keys to string values; unquoted `0.1.5` survived only because two dots make it unparseable as a number, and the first two-part version would have been silently coerced to a float.
- **README reorganized** from "the three companion files" to what the repository actually contains now, separating the loaded protocol from the on-demand references.

**Why**

`SKILL.md` had reached roughly 12,000 tokens — about 2.4× the ~5,000-token budget the Agent Skills guidance recommends for a skill body. It passed the 500-line ceiling only because its lines are dense prose rather than code. Every one of those tokens loaded on invocation and then competed with the user's actual work, which matters more here than for most skills: this protocol is meant to govern a long working session, not a single transformation.

Reviewing the file against the published guidance surfaced a structural problem underneath the size one: it was serving two audiences at once. Most of it governs a model at runtime, but the contribution machinery addresses human contributors, and the crack registry is field evidence rather than instruction. Splitting by audience — what a model acts on, versus what a person reads when deciding whether to trust or amend the protocol — is what made the cut possible without losing anything.

**Decision recorded**

The cut stops at 8,870 tokens rather than reaching the recommended 5,000. Getting under that number would mean compressing §3.5, §6, §7, and §9.5 — the calibration-heavy sections — into terse bullet stubs, and the protocol has direct evidence that this fails: Crack 004 is what happened when the machinery became salient and got printed as headers instead of run. Terse mechanical rules invite exactly that. Extraction of reference material is the safe lever; compressing judgment calibration into fragments is not. If a smaller footprint is needed later, the answer is a separate lite edition, not a thinner canonical file.

**Origin artifact**

Review of `SKILL.md` against the Agent Skills authoring guidance and format specification, 2026-08-17, prompted by a question about whether the file followed current best practice. The routing-table and layered-loading patterns were adopted after examining an unrelated file-based protocol kit that uses a symptom-to-file dispatcher and one-topic-per-file modules; only those two structural patterns were taken, and its telegraphic compression style was explicitly rejected for the reason recorded above.

---

## 2026-08-17 — v0.1.5 — README: IT/security-reviewer framing + layer-placement

**What changed**

- **New README section — "For IT / security review"** at the top of the file, above the conceptual body: nothing to install, stateless, no attack surface of its own, fully readable and forkable. It front-loads facts that already existed rather than adding new ones.
- **New README section — "Where this sits"** naming a three-layer stack — IT/platform governance above, AI awareness and literacy below, authorship and decision governance in the middle — and placing this protocol in the middle layer explicitly as non-competing with existing controls.
- **§15 reconciled, not duplicated.** The stateless bullet is now the single canonical statement (extended to cover "no external calls, collects no data" so it is never narrower than the README's summary), and the README cross-references it instead of restating it. The passing mention of statelessness in the README's "How to use it" section was cut for the same reason.
- **Version bump** to 0.1.5.

**Why**

The repository travels on its own, and its realistic path is to be forwarded — from someone sympathetic to a team who reads anything entering their environment adversarially. That reader asks four questions first: what does this touch, collect, or transmit; is it a policy, a control, or a philosophy; where does it sit relative to controls we already run; and does adopting it cost us anything to secure. The answer to the first already lived in §15, but an IT reviewer does not read to §15. The failure was placement, not content: if the top of the README doesn't defuse the attack-surface question, the body never gets read.

The second addition answers a different reflex — filing an "AI governance" artifact as a redundant or competing policy that overlaps an existing acceptable-use policy or approved-tool list. Naming the layer makes the protocol legible as an authorship standard rather than an engineering control, which is also the standing answer to the recurring misread of this method as human-in-the-loop: HITL lives in the top layer, and this does not.

**Decision recorded**

Facts that decide whether the repository gets read at all belong at the top, and they belong in one place. The protocol is placed as the middle layer of a three-layer stack — it assumes tool-and-data governance exists and governs the human decision at the point of use, which no tool-and-data control can specify. It stays non-prescriptive: it describes a layer, it does not mandate organizational policy. The layer framing also carries a practical consequence worth stating — because the unit of governance is one person at the point of use, an organization can apply consistent authorship standards without waiting on a finalized global policy.

**Origin artifact**

Internal handoff spec, 2026-08-17: an analysis of how the repository is actually received when read cold by a reviewer assessing it as an artifact entering their environment, rather than warmly by a reader already interested in the method. Two README sections were specified; the prior-art section ("isn't this just HITL, red teaming, or dialectic?") and Crack 007 were deliberately held back as separate edits.

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
