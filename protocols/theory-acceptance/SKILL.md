---
name: theory-acceptance
description: Decide whether a proposed scientific definition or theory result 
is mature enough to become canonical theory. 
Use after theory construction and independent review, 
before implementation or release is treated as authoritative.
---

# Theory Acceptance

Use this protocol to decide whether a theory result may move from candidate
status to canonical theory.

This is a scientific acceptance gate.

It is not a code-completion checklist.

## Core Rule

A theory result is accepted only after it survives a test that could have
rejected or narrowed it.

Plausibility, implementation success, and reviewer confidence are insufficient.

## Acceptance Inputs

The acceptance packet should contain:

- the candidate definition or theorem;
- settled background;
- source-audit result where relevant;
- explicit assumptions;
- known exclusions;
- adversarial tests;
- independent review reports;
- unresolved/deferred ledger;
- proposed canonical wording.

## Gate A. Semantic Precision

The candidate must state:

- its domain;
- its intended meaning;
- its polarity where applicable;
- relevant parameters or scope;
- what it excludes;
- its relationship to adjacent concepts.

A definition that requires the reader to infer its operative meaning remains
OPEN.

## Gate B. Counterexample Resistance

The candidate must have been tested against concrete pressure cases.

At least one review must actively attempt rejection.

If a valid unresolved counterexample remains, the result is OPEN.

## Gate C. Source Compatibility

Where the result extends an existing theory:

- identify what is preserved;
- identify what is strengthened;
- identify what is revised;
- identify any current interfaces that are intentionally weaker.

Do not call new semantics a recovery of old semantics.

## Gate D. Independence

At least one substantive adversarial review must have been performed without
seeing the author's full reasoning path.

For high-impact foundation changes, prefer two independent reviews.

## Gate E. Boundary Integrity

Confirm that the candidate does not accidentally collapse concepts that the
theory requires to remain distinct.

Typical checks:

- truth versus evidence;
- identity versus equality;
- same-unit versus parthood;
- denotation versus co-reference;
- individuation versus persistence;
- foundational commitment versus attributed claim.

## Gate F. Deferred Issues

Every adjacent unresolved issue discovered during the work must be either:

- resolved;
- shown not to affect acceptance;
- explicitly deferred with a reason.

No unresolved dependency may be hidden by omission.

## Gate G. Human Review

Before canonical adoption, a human reviewer must inspect:

- the final candidate;
- the strongest counterexample attempted;
- all accepted narrowings;
- the canonical wording.

Agent consensus alone cannot close the gate.

## Verdicts

Use exactly one:

### OPEN

The scientific result is not ready for canonical adoption.

### ACCEPTED WITH RECORDED LIMITS

The core result is accepted, with explicit scope or exclusions that remain part
of the definition.

### ACCEPTED

The current scientific question is sufficiently resolved for canonical theory.

Acceptance does not imply that all downstream consequences are resolved.

## After Acceptance

Only after acceptance should the project proceed to the next approved stage,
for example:

- canonical prose;
- Lean formalization;
- reference artifact updates;
- downstream interface analysis;
- specification propagation;
- release preparation.

Do not combine scientific acceptance and implementation into one unreviewed
step.

## Failure Modes

- Accepting because the implementation builds.
- Accepting because two agents agree.
- Hiding a narrowing in commentary rather than the definition.
- Treating an unresolved adjacent issue as irrelevant without analysis.
- Letting downstream dependencies dictate upstream semantics.
- Editing the canonical source before the acceptance decision is inspected.

## Completion Condition

The gate closes only when:

- the semantic contract is explicit;
- adversarial review could have failed it;
- remaining limits are recorded;
- independent review is complete;
- human inspection has occurred.

## Sources and Acknowledgments

This protocol is informed by the acceptance-gate discipline used by BootLoops:
define completion externally, require a check capable of failure, preserve
honest OPEN outcomes, and distinguish production from certification.

The quantitative BootLoops acceptance criteria are not adopted here;
this protocol specializes the general discipline for formal and semantic theory.

See `reference/upstream.toml` for pinned upstream provenance.
