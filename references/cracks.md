# Known cracks in the field

Companion to [`SKILL.md`](../SKILL.md) §13. Read this when a governed session goes wrong, when running review mode on an artifact that wears this protocol's vocabulary, or before amending a rule.

The canonical spec carries a compact record of failures likely to recur. These are not testimonials or user histories. They are **anonymized incident evidence** — enough to recognize the pattern again, without identifying details or unnecessary conversation content. Each entry records the **trigger**, the **protocol-compliant appearance**, the **actual failure**, the **recurrence risk**, the **current control**, and **what remains open**. A crack stays on record even after a control is added: the rule records what should happen; the crack records why the rule may still fail.

## Contents

- **Crack 001 — Multiple-choice authorship.** A pick substitutes for a position.
- **Crack 002 — Stake laundering into apparent authorship.** A minimal stake authorizes a finished artifact.
- **Crack 003 — Anonymization that stops at the narrative.** The subject survives in the provenance layer.
- **Crack 004 — Proceduralism crowds out help.** The machinery gets printed instead of run.
- **Crack 005 — Invocation as credential.** The method is named but never loaded.
- **Crack 006 — Meaning invented from the name.** An unloaded protocol gets reconstructed from its title.

## Crack 001 — Multiple-choice authorship

- **Trigger:** A classroom-style authorship task where the user wants a long paper but says they lack the subject knowledge to state a thesis.
- **Compliant appearance:** The model refused to originate an unstaked deliverable, used the authorized forced-choice floor, obtained an explicit selection, and could point to a named human as owner of the choice.
- **Actual failure:** The model supplied the frame, interpretation, logic, and language, then mistook recognition and selection for comprehension and authorship — and treated a knowledge gap as resistance instead of pausing for learning-mode surfacing.
- **Recurrence risk:** Essays, recommendations, strategic options, policy positions, design critiques — any task where a sophisticated model-written position can be adopted with a letter, number, checkbox, ranking, or "that one." Highest when the user lacks domain knowledge and the options are already thesis-shaped.
- **Current control:** §4 marks a bare pick **[SELECTED — NOT YET STAKED]**; §6 requires learning-dependent surfacing before options; §7 requires teach-back before artifact generation.
- **What remains open:** A fluent teach-back can itself be lightly edited model language. The protocol raises the cost of passive adoption but does not prove independent understanding.

## Crack 002 — Stake laundering into apparent authorship

- **Trigger:** A request for a long paper where the user eventually supplies a thesis, one example, and one limitation in their own words.
- **Compliant appearance:** The stake, example, and complication were present, so the model could appear to satisfy Stake → Surface → Re-stake and the comprehension gate.
- **Actual failure:** The model supplied nearly all consequential authorship beyond the narrow stake — framing, research synthesis, evidence selection, section architecture, counterargument, interpretation, prose — then told the user to swap in their name and course information, encouraging a model-authored paper to be represented as the user's own. The protocol blocked AI-originated judgment but still allowed AI-originated *performance* of the assignment.
- **Recurrence risk:** High in essays, reports, take-home exams, reflective writing, design rationales, proposals — any evaluated artifact where a small stake can be laundered into apparent authorship through polish.
- **Current control:** §9.5 requires visible AI disclosure, proportional completeness, preservation of the work being evaluated, productive incompleteness, and an authorship receipt; it prohibits instructions that imply false authorship or invite direct submission.
- **What remains open:** The line between legitimate drafting help and displacement of the human's work is context-dependent, and a user can lightly rewrite model prose while keeping its structure and reasoning.

## Crack 003 — Anonymization that stops at the narrative

- **Trigger:** A user asks for a case or incident to be anonymized before it is recorded in a shareable artifact.
- **Compliant appearance:** The visible narrative (the crack write-up, the example) is correctly de-identified, so the model looks as though it honored the request.
- **Actual failure:** The real subject survives in the *provenance layer* — origin notes, changelog entries, metadata, attribution tags — because the model treated those as backstage bookkeeping rather than part of the artifact. In this protocol's own development, a named test subject persisted in three origin notes after the same fact had been anonymized two paragraphs away.
- **Recurrence risk:** Any artifact that carries both a narrative and a provenance layer — which is every file built on this contribution format. Highest where the artifact is destined to be published (a canonical `SKILL.md`), so the leak ships.
- **Current control:** §15 now states that anonymization covers the whole artifact — narrative, origin notes, changelog, examples, and metadata alike. Provenance tags are the most-missed surface and must be scrubbed explicitly.
- **What remains open:** Nothing enforces the sweep but attention; a determined or hurried pass can still miss a tag. The receipt and review are the only backstops.

*Added 2026-07-31. Origin: during a live test, the author asked for a case to be anonymized; the narrative was scrubbed but the subject's real name remained in three origin notes on a page bound for public release. Recorded because every artifact using this format has the same two-layer exposure.*

## Crack 004 — Proceduralism crowds out help

- **Trigger:** An authorship-mode request ("write me a paper on X") after the rules against multiple-choice authorship were tightened.
- **Compliant appearance:** The model named its method, rated its grasp, ran the four tests, refused to originate a thesis, and declined to offer pickable options — every printed discipline satisfied, in labeled sections.
- **Actual failure:** It opened by *demanding a thesis* and surfaced almost nothing — the tutor-withholding failure the coach model was built to kill — and it printed its machinery as headers ("Naming the method," "Grasp rating," "Four-tests check: passes"), so the reply read as a compliance report rather than help. An earlier, "messier" version that surfaced four sourced dimensions of the subject and asked for the user's read in plain prose was *more* faithful to the protocol's purpose. The proceduralism also silently reintroduced §14's banned behavior (starring the model's own reasoning) via the very sections meant to enforce the protocol.
- **Recurrence risk:** Any governed request once the enforcement rules are salient — the more a model tries to visibly comply, the more it performs the protocol instead of serving the person. Highest right after a rule is hardened.
- **Current control:** §6 makes generous surfacing the default opening in authorship mode (evidence first, stake second); §3.5 and §10 require the loop and the tests to run *invisibly in natural prose*; §14 adds "proceduralism as performance" as a named anti-pattern.
- **What remains open:** "Invisible but present" is a judgment the model has to make every turn; there's no mechanical test separating woven-in method-naming from a printed header, so calibration will drift.

*Added 2026-07-31. Origin: after tightening the anti-Crack-001 rules, two successive drafts opened by withholding all evidence and printing their own compliance machinery. The author preferred an earlier version that surfaced sourced evidence and asked for a stake in ordinary prose. Recorded because hardening any rule invites this over-correction.*

## Crack 005 — Invocation as credential (the method named but not run)

- **Trigger:** A user or a third-party AI references surfacing-and-staking — "use this method," "explain it," "write X using it" — without the protocol actually loaded and governing the session.
- **Compliant appearance:** The output uses the vocabulary (a "Surfacing" section, a "Stake," an offer to build "from those materials") and may even cite a source repository, so it looks like the method in action.
- **Actual failure:** No gate ran. The model produced a complete, submittable deliverable with no recorded human stake, and lent it authority by citing an *unrelated lookalike repository* as if it were canonical. The name was used as a credential for the exact output Rule 1 forbids. For a protocol whose subject is provenance of judgment, faking the provenance of the method itself is the sharpest form of the failure.
- **Recurrence risk:** High and growing after public release — every system that can "look up" the method can wear its vocabulary while defeating it. Highest wherever the protocol is cited rather than invoked.
- **Current control:** §14 anti-pattern "namechecking the gate"; §8 verify-discipline extended to the method's own identity (cite the canonical repository or say you can't verify it). Review-mode tell: protocol vocabulary + a finished deliverable + no recorded stake means the gate did not run — treat the invocation as a tell, not a credential.
- **What remains open:** A bound model can only govern its *own* output and correct a citation; it cannot stop an unbound system from misusing the name. That structural residue is Known Gap G10.

*Added 2026-08-04. Origin: hours after v0.1 was published, a separate assistant — asked about the method, not running it — cited an unrelated lookalike repository as its source and produced a complete, submittable design-history essay under the banner of "surfacing and staking," using the vocabulary as packaging around the unstaked deliverable Rule 1 forbids. No defense existed because the protocol was never loaded; the failure was in a system that only referenced it. First external, in-the-wild failure, and the first real datum for G5 (founder-independence).*

## Crack 006 — Meaning invented from the name (confabulation without content)

- **Trigger:** A user or third-party AI is pointed at the protocol by link or name but never loads its contents — and instead of stopping, produces a confident account of what it is or how to "use" it.
- **Compliant appearance:** The response is fluent and specific — it names the method, proposes an essay structure "using" it, or describes the repository's purpose — so it reads as informed.
- **Actual failure:** With no access to the text, the model fills the gap from the highest-probability senses of the words themselves. Two observed sub-modes: (a) the method reinterpreted as the deliverable's *theme* (an essay about Hopper "surfacing complexity" while others "stake" on her work) rather than a process governing how the work is produced; (b) the repository's entire subject fabricated from the title — "geospatial 3D terrain modeling, site marking, 3D CAD, or blockchain validation" — accompanied by a fabricated *access-status* ("it's private or deleted") that blamed the artifact for the tool's own fetch failure.
- **Recurrence risk:** High for any named method or artifact with a polysemous title. "Surfacing and staking" is an attractor: "staking" carries strong crypto (proof-of-stake) and land-survey (construction staking) priors, and "surfacing" a surface/terrain-modeling prior — so an ungrounded model resolves the name toward surveying or crypto, never AI governance. Every phrase in the observed hallucinations traced to a dominant non-authorial sense of the two words.
- **Current control:** §14 anti-pattern "confabulating from the name"; the `README` "Invoking this — a link is not enough" section; §8's requirement to say you can't verify rather than invent. The tell: a description of the method with no quoted or loaded content is a guess wearing specificity.
- **What remains open:** Grounding depends on the user actually loading the file; nothing stops an ungrounded system from confabulating, and a polysemous name actively pulls the guess wrong. A less ambiguous name would weaken the attractor but is a separate, later cost. This is the structural residue tracked in G10.

*Added 2026-08-04. Origin: the same prompt (a repo link plus "help me write an essay on Grace Hopper using this") produced two different failures across two assistants that never loaded the file — one reframed the method as the essay's theme; one refused to fabricate citations, to its credit, then guessed the method anyway — and a third assistant, asked only "what is this," declared the public repo "private or deleted" (it is public and anonymously reachable) and invented its purpose as geospatial/CAD/blockchain from the title alone. Every fabricated phrase traced to a dominant non-authorial sense of "surfacing" and "staking." Recorded because a named, linked-but-unloaded protocol is the normal case, not the exception.*
