---
name: theory-construction
description: Develop or revise scientific theory when the correct 
semantics, definitions, or structure are not yet settled. 
Use when the task is theory-finding rather than 
proving or implementing an already established statement.
---

# Theory Construction

Use this protocol when the scientific object itself is under construction.

The goal is not to preserve the current implementation.
The goal is to identify a coherent scientific semantics that can later be
formalized, tested, and implemented.

## Core Rule

Separate:

- what is already established;
- what is currently unspecified;
- what is being proposed;
- what remains unresolved.

Do not present a proposed semantic commitment as though it were recovered from
an existing specification or implementation.

## Procedure

### 1. State the scientific question

State exactly one primary question.

Examples:

- What does individuation mean?
- What distinguishes individuation from persistence?
- What conditions make two regimes scientifically distinct?
- What must a denotation relation establish?

Avoid beginning with a preferred formal representation.

### 2. Freeze established background

List only facts already supported by
authoritative theory, source material, or
prior accepted results.

Identify:

- established definitions;
- explicit non-assumptions;
- relevant invariants;
- known counterexamples;
- deferred issues that must not be reopened.

### 3. Identify the semantic gap

State what the current theory does not determine.

Distinguish:

- missing semantics;
- deliberate abstraction;
- implementation omission;
- contradiction;
- unresolved design choice.

Do not infer positive semantics from silence.

### 4. Propose one candidate

State one coherent candidate strongly enough to be falsifiable.

A candidate should specify, where relevant:

- domain;
- polarity;
- intended meaning;
- exclusions;
- relationships to adjacent concepts;
- consequences that would follow if accepted.

Do not offer multiple alternatives unless comparison among alternatives is the
scientific question.

### 5. State what the candidate does not claim

Explicitly protect neighboring concepts from accidental collapse.

Typical distinctions include:

- semantic truth versus evidence;
- identity versus identifier equality;
- individuation versus co-reference;
- individuation versus persistence;
- reference resolution versus interpretation;
- parthood versus same-unit identity;
- foundational commitment versus attributed claim.

### 6. Construct adversarial tests

Try to break the candidate.

Use:

- concrete counterexamples;
- boundary cases;
- examples from each affected carrier or domain kind;
- algebraic consequences;
- circularity tests;
- neutrality tests;
- comparison with authoritative source language.

A rejection must identify a scientific failure,
not merely the absence of a
current implementation.

### 7. Require a verdict

Use one of:

- ACCEPT
- ACCEPT WITH NARROWING
- REJECT
- FUNDAMENTAL QUESTION REMAINS

For ACCEPT WITH NARROWING, state the smallest exact narrowing.

For REJECT, provide the counterexample or contradiction that forces rejection.

### 8. Preserve the deferred ledger

Record adjacent issues discovered during the analysis without allowing them to
take over the current question.

Each deferred issue should have:

- a short identifier;
- one-sentence description;
- reason it is deferred.

### 9. Record the converged definition

When a candidate survives review, write the strongest concise scientific
definition supported by the analysis.

Do not implement it yet unless implementation is the next explicitly approved
stage.

## Failure Modes

- Reading semantics back out of an intentionally weak interface.
- Letting the current type signature dictate the science.
- Treating lack of evidence as semantic negation.
- Treating a reviewer preference as a counterexample.
- Broadening into adjacent unresolved topics.
- Repairing implementations while the scientific definition is still moving.
- Calling a theory settled because several agents found it plausible.

## Completion Condition

Theory construction is complete for the current question when:

- the semantic question has a clear answer;
- the candidate survived concrete adversarial tests;
- necessary narrowings are explicit;
- neighboring concepts remain distinct;
- unresolved issues are on the deferred ledger;
- independent review has not produced an unresolved counterexample.

The result is then eligible for the theory-acceptance protocol.

## Sources and Acknowledgments

This protocol is informed in part by the adversarial, falsification-oriented,
and theory-finding workflow in the BootLoops research protocols, especially
`prove-protocol`,
but is specialized for semantic and formal theory
construction in Structural Explainability.

See `reference/upstream.toml` for pinned upstream provenance.
