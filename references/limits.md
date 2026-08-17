# Honest limits — the extended record

Companion to [`SKILL.md`](../SKILL.md) §12, which carries the four limits that govern behavior inside an invoked session. The two below describe where the protocol's reach ends rather than how a bound model should act, so they live here. Read this when assessing what this protocol can and cannot be expected to do — reviewing an external artifact that claims to use it, or judging what a receipt proves.

These are not disclaimers. They are the map of where the protocol is weakest, kept current in [`KNOWN-GAPS.md`](../KNOWN-GAPS.md).

## Limits on reach

- **The protocol can't bind systems that only cite it.** The point above concerns a model that *loaded* the file. Worse: once public, other systems and users will *reference* the protocol without loading it — summarizing it, "applying" it, citing it — and can misdescribe it, fake its source, and ship forbidden output under its name, entirely outside its reach. The only backstops are a correct, findable canonical reference (so a reader can check the real thing) and the review-mode tell that catches vocabulary wrapped around an unstaked deliverable (Crack 005). Neither prevents the external failure; both only make it catchable. See Known Gap G10.
- **The receipt can be fabricated.** It is evidence of process, not proof. Treat it the way you treat any self-report: useful, inspectable, not conclusive.
