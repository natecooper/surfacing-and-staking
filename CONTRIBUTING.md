# Contributing

This protocol improves the way the best-known behavioral files improved: someone gets frustrated enough to be precise about what went wrong, and the fix becomes a rule with a story attached. Finding a bypass is a first-class contribution, not a violation. The arms race is the development model, run in the open.

Start with [`SKILL.md`](SKILL.md) §13 for what to do the moment a gate fails, and [`references/cracks.md`](references/cracks.md) for the failures already on record — check there before filing, since a new specimen of an existing crack belongs in that entry rather than in a new one.

## Filing a crack

If you routed around the gate, file it as a [`KNOWN-GAPS.md`](KNOWN-GAPS.md) entry: what you said, what the model did, and which rule failed. Include enough to reproduce the pattern and nothing more.

## Rule format

Every new or amended rule carries an origin:

```
Rule text (imperative, short).
*Added [date]. Origin: [the specific failure that created this rule —
what happened, why the old text didn't hold, what the fix changes].*
```

Rules without origin stories don't get merged. The origin is the evidence; the rule is the stake.

Keep origin notes in `SKILL.md` short and attached to the rule they justify. The full incident record belongs in [`CHANGELOG.md`](CHANGELOG.md), which is the protocol's own re-stake record — every merged change earns an entry.

## Anonymization

Anonymization covers the whole artifact — narrative, examples, origin notes, changelog entries, attribution, and metadata alike, per `SKILL.md` §15. The provenance layer is the most-missed surface and must be scrubbed explicitly. Verify it is clean before publishing anything bound for release. This is Crack 003; the format used here has that exposure by construction.

## Adaptations

Adaptations are encouraged — a classroom edition, a clinical edition, a newsroom edition. Label adaptations as adaptations, keep the section-status labels honest, attribute per the license, and file what you learn upstream.

## Section statuses

**stable** = current canonical position · **working** = coherent, expected to change through use · **draft** = partly specified, needs testing. Keep these honest when amending a section; a status that no longer matches the text is its own defect.
