# Known Gaps

What's broken, under-defined, or unproven in the protocol — kept honest and current. **Finding a new crack (including routing around the gate) is a first-class contribution, not a violation.** File what you find here, with the story of how it broke.

## Open gaps (v0.1)

### G1 — A text file cannot jail-proof a model *(severity: structural, permanent)*

Sustained pressure, clever reframing, or simply closing the file defeats every rule. The design goal is not "uncircumventable" but "circumvention is louder than compliance" — the receipt is meant to make a bypass visible after the fact. **Still unproven:** whether the receipt tell actually deters, or is just legible to someone already looking.

### G2 — The AI administering the framing is itself a framing risk *(severity: high)*

The protocol asks the model to run the gate, and a model can smuggle a verdict while obeying the letter of the rules. The tell is output that stars the AI's reasoning and ends in a recommendation. **The reliable check is the human catching it, not the rule preventing it** — which means the protocol leans on the very vigilance it's trying to supply. Not yet resolved.

### G3 — The triage boundary is a judgment call *(severity: medium)*

§5 says the protocol fires only when "someone will have to own an outcome," but that line is fuzzy at the edges (is a first-draft brainstorm a judgment? a study outline?). Too broad and it becomes governance theater that gets uninstalled; too narrow and it misses real stakes. Needs sharpening through use.

### G4 — The receipt can be fabricated *(severity: medium)*

It's evidence of process, not proof. An instructor requiring receipts will eventually receive an invented one. Open question whether anything short of session logging (explicitly out of scope, §15) can raise the cost of faking without breaking statelessness.

### G5 — Founder-independence unproven *(severity: high, until tested)*

v0.1 has not been demonstrated to work in a fresh session without its author in the room. Until it runs clean for someone else, every "it works" is untested. **Partial evidence:** live cross-model tests (a separate assistant, with only the page as instruction) produced faithful behavior after the v0.1.2 fixes — the strongest sign yet, but still author-in-the-loop since the author ran and judged them.

### G6 — When does facilitation end? *(severity: medium — partially addressed v0.1.1)*

The coaching loop (§3.5) originally had no hard boundary for "the problem is now defined well enough." **v0.1.1 added the five-whys hard stop:** five rounds on one line with no stake → hard-stop that line and pivot; a second exhausted line → stop facilitating entirely, record non-readiness as the honest finding, optionally offer cited reading. This bounds the loop and kills the infinite-recursion path. **Still open:** the count (five, then one pivot) is asserted, not tested; and a determined user could still stall inside a single line short of five. Sharpen through use.

### G7 — Stated confidence is a persuasion surface *(severity: high)*

Any stated confidence carries weight, and models are miscalibrated — a confident-sounding rating can manufacture the agreement it's meant to inform. **v0.1.1 split the two ratings:** the coach's *problem-grasp* (§3.5) stays plain-language (a number there only nudges); *output-confidence* (§8) is a percentage *because* it's bound to a verify mandate, citations, a >75% "how confident are you?" challenge, and a <50% harsh warning — so the number triggers scrutiny, not agreement. **Still open:** the split reduces the nudge but doesn't remove it, and a miscalibrated percentage is still a persuasion surface even when paired with a challenge. The 50–75% band is intentionally quiet (proceed + standing verify reminder) — watch whether that band gets rubber-stamped.

### G8 — A human stake can be laundered into apparent authorship *(severity: high)*

The protocol originally treated a sufficiently understood human claim as the key threshold for artifact generation. A second authorship-mode test showed that this is not enough. A user can contribute a real but very small stake while the model supplies nearly all of the structure, evidence selection, interpretation, and prose. The resulting artifact may then look human-authored even though the human performed little of the work the assignment was intended to exercise.

**Current control:** §9.5 adds authorship disclosure, proportional artifact completeness, productive incompleteness, preservation of the human work being evaluated, and a prohibition on submission-oriented instructions such as "add your name and turn it in." Crack 002 records the incident in the canonical field registry.

**Still open:** No general rule yet determines how much human contribution is enough for each artifact type. Disclosure can reveal provenance but cannot guarantee that the person performed the intended thinking. Light human rewriting may also preserve model-originated structure and reasoning while creating the appearance of authorship. This boundary must be sharpened through classroom, workplace, and publication tests.

### G9 — Enforcement machinery crowds out help *(severity: high)*

The more visibly a model tries to comply with the protocol, the more it performs the protocol instead of serving the person. Two live authorship-mode tests opened by withholding all evidence and printing the machinery as labeled headers ("Naming the method," "Grasp rating," "Four-tests check: passes") — satisfying every printed discipline while failing the purpose. A "messier" version that surfaced sourced evidence and asked for a stake in plain prose was more faithful.

**Current control:** §6 makes generous surfacing the default opening; §3.5 and §10 require the coaching loop and four tests to run invisibly in natural prose; §14 adds "proceduralism as performance"; Crack 004 records it.

**Still open:** "Invisible but present" is a per-turn judgment with no mechanical test — nothing cleanly separates woven-in method-naming from a printed header, so calibration will drift, and hardening any future rule invites the same over-correction again.

### G10 — The protocol can't bind systems that only cite it *(severity: high, structural)*

§12 already admits a text file can't jail-proof a model that *loaded* it. G10 is the worse, permanent version: once public, other AIs and users will *reference* the protocol without loading it — summarizing it, "applying" it, citing it — and can misdescribe it, cite a fake source, and ship forbidden output under its name, entirely outside its reach. The only backstops are a correct, findable canonical reference (so a reader can check the real thing) and the review-mode tell (Crack 005) that catches protocol vocabulary wrapped around an unstaked deliverable. Neither prevents the external failure; both only make it catchable after the fact.

**First observed 2026-08-04** (see Crack 005): hours after publication, a separate assistant asked about the method cited an unrelated lookalike repository and produced a complete, unstaked essay under the protocol's banner. This is also the first in-the-wild datum for G5 — the founder was still in the room, but the failing system was not the author's.

**Two more specimens, same root (2026-08-04, see Crack 006):** a second assistant given "help me write an essay using this repo" reinterpreted the method as the essay's *theme* rather than a process; a third, asked only "what is this," reported the public repo as "private or deleted" and invented its purpose — "geospatial 3D terrain modeling, site marking, 3D CAD, or blockchain validation" — from the title alone. Verified counter-fact: the repo is public and anonymously reachable (HTTP 200), so the access-status was fabricated. **The name is an attractor:** "staking" carries strong crypto (proof-of-stake) and land-survey (construction staking) priors, "surfacing" a surface/terrain-modeling prior — every hallucinated phrase traced to a dominant non-authorial sense of the two words. When the file isn't loaded, the name *is* the entire prior, and this one points away from AI governance. **One bright spot (§8 working):** the second assistant refused to fabricate citations and asked for the source before guessing content — the honest branch §8 prescribes. The `README` "Invoking this — a link is not enough" section is the current mitigation; a less polysemous name would weaken the attractor, at a separate cost.

---

*Every live test seeds a real entry. Running the protocol in a fresh session — where it holds vs. where it's talked out of the gate — becomes the next gap. G6–G9 all came from live tests this way.*
