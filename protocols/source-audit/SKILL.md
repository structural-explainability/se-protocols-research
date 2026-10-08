---
name: source-audit
description: Determine what existing authoritative sources actually 
define, require, omit, or leave unresolved. 
Use before changing theory when the question 
is whether a semantic claim already exists in papers, 
specifications, formalizations, registries, or repository artifacts.
---

# Source Audit

Use this protocol to answer:

> What do the existing sources actually establish?

The purpose is recovery and classification, not repair.

## Core Rule

Report the source as it is.

Do not silently:

- improve it;
- reconcile conflicting sources;
- infer missing definitions;
- promote comments into laws;
- treat implementation behavior as normative unless authority says so.

## Procedure

### 1. State the audit question

Use one focused question.

Examples:

- What does `individuationConditions` mean?
- Is carrier equality assigned semantic force?
- Where is reference denotation defined?
- Does the theory assume co-reference reflexivity?
- Which artifact owns this requirement?

### 2. Declare the authority order

Before interpreting conflicting artifacts, identify which sources are
authoritative for which claims.

Possible source classes include:

- normative paper;
- specification;
- Lean formalization;
- reference registry;
- manifest;
- implementation;
- README;
- generated artifact;
- historical notes.

Do not assume one global authority order if different artifacts own different
surfaces.

### 3. Record source coverage

List:

- sources inspected;
- relevant files;
- relevant modules or sections;
- sources known but unavailable or unread.

An unread source must not be treated as confirming the audit result.

### 4. Extract explicit commitments

For each relevant source, classify statements as:

- definition;
- axiom or requirement;
- theorem;
- declared non-assumption;
- descriptive prose;
- implementation choice;
- example;
- historical artifact.

Preserve the source's terminology.

### 5. Search for relationships, not only names

If auditing concept A, also inspect whether the source defines relationships
between A and adjacent concepts.

Examples:

- individuation ↔ co-reference;
- identity ↔ equality;
- persistence ↔ transformation;
- reference ↔ carrier;
- proposition ↔ attribution.

Absence of a relationship is itself relevant only when the search scope is
adequate.

### 6. Distinguish four outcomes

Use these categories:

A. FOUND

The requested semantic contract is explicitly present.

B. PARTIAL

Relevant pieces exist, but the requested contract is incomplete.

C. NOT FOUND

The searched authoritative surfaces do not contain the requested contract.

D. UNDER-SPECIFIED

The theory deliberately permits multiple semantic realizations or leaves the
question unresolved.

Do not use NOT FOUND when the real result is simply NOT READ.

### 7. Separate recovered truth from new proposal

End with two sections:

- JUSTIFIED FROM CURRENT SOURCES
- WOULD REQUIRE NEW THEORY OR INTERFACE

Never mix them.

### 8. Name exactly one next question

If the audit exposes a gap, state the smallest next scientific question.

Do not automatically design the repair.

## Failure Modes

- Treating comments as stronger than formal declarations.
- Treating a missing theorem as evidence that its converse holds.
- Conflating code-level equality with semantic identity.
- Using downstream assumptions to define upstream semantics.
- Declaring architectural intent from chronology alone.
- Searching until a desired interpretation appears.
- Repairing the source during the audit.

## Completion Condition

A source audit is complete when another reviewer can tell:

- exactly what was searched;
- which sources carry authority;
- what is explicitly supported;
- what is absent or under-specified;
- what remains unread;
- what would require new theory.

## Sources and Acknowledgments

This protocol is informed by the source-discipline and reading-contract ideas
in the BootLoops research protocols, adapted for multi-repository formal
theory systems.

See `reference/upstream.toml` for pinned upstream provenance.