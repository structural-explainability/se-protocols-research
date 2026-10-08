---
name: referee-sim
description: Simulate strong external review of an SE paper, 
theory release, specification, or major scientific claim 
before circulation. 
Use when the work is internally coherent 
but needs testing against the objections 
an informed outside reader is likely to raise.
---

# Referee Simulation

Use this protocol before circulating an outward-facing scientific artifact.

The purpose is not to repeat internal verification.
The purpose is to test what an informed external reader is likely to challenge,
misunderstand, or infer from the presentation.

## Core Rule

Audit both:

- whether the claims are correct;
- whether the document frames their scope and novelty correctly.

A document can be technically true and still create a false scientific
impression.

## Procedure

### 1. Identify relevant audiences

List the communities whose standards the artifact invokes.

Include:

- formal methods or theorem-proving readers;
- software engineering researchers;
- domain researchers whose examples or terminology are used;
- incumbent theory or method communities;
- empirical or verification communities where evidence is claimed;
- the venue's general technical reader.

Only include audiences genuinely implicated by the artifact.

### 2. Generate the strongest standard objection

For each audience, generate at least:

- one correctness/scope objection;
- one novelty/positioning objection where novelty is claimed.

The objection should be one a competent skeptical reviewer could plausibly
lead with.

Avoid exotic objections that distract from the standard first-order concern.

### 3. Steelman the objection

The objection must identify:

- the assumption being challenged;
- the source of the concern;
- the scientific consequence if the objection succeeds.

Weak objections that the document already trivially answers provide little
value.

### 4. Check the reader's path

Determine where the artifact answers the objection.

Important limitations should appear before the reader forms a stronger
impression.

Check especially:

- title;
- abstract;
- introduction;
- headline figures;
- theorem statements;
- conclusions;
- scope sections.

An answer buried elsewhere may not adequately control the claim.

### 5. Audit claim status

Check language such as:

- proves;
- establishes;
- guarantees;
- necessary;
- sufficient;
- complete;
- minimal;
- first;
- general.

Confirm the stated status matches the evidence.

Distinguish:

- theorem;
- conjecture;
- proposed semantics;
- empirical observation;
- design choice;
- compatibility result;
- negative result.

### 6. Check internal scientific boundaries

For SE artifacts, pay special attention to accidental collapse among:

- substrate and interpretation;
- reference and referent;
- individuation and persistence;
- identity and equality;
- attributed claim and foundational commitment;
- preservation and completeness;
- generated relation and stipulated classification.

### 7. Run in a fresh context

The referee simulation should not be performed by the same agent context that
authored the artifact.

The reviewer should receive the artifact and necessary sources, not the
authoring discussion.

### 8. Produce a referee table

Record:

- audience;
- objection;
- correctness or novelty;
- severity;
- where answered;
- whether a change is required.

Use severity:

- HIGH: could invalidate or materially misstate the main claim;
- MEDIUM: claim is supportable but framing or scope is misleading;
- LOW: clarity or positioning improvement.

### 9. Make minimal corrective changes

Prefer:

- precise scope statements;
- explicit status labels;
- stronger source attribution;
- moving an existing limitation to where readers need it;
- narrowing an overbroad claim.

Do not respond to review by weakening every sentence indiscriminately.

## Failure Modes

- Friendly simulated referees.
- Reviewing in the authoring context.
- Generating objections only from the project's own vocabulary.
- Checking correctness but not novelty.
- Treating a buried caveat as sufficient.
- Replacing a precise claim with vague hedging.
- Claiming consensus because no reviewer was asked a difficult question.

## Completion Condition

Referee simulation is complete when:

- relevant audiences are represented;
- their strongest standard objections have been recorded;
- high-severity objections are answered or the claims are narrowed;
- claim status is accurate;
- the review occurred in a fresh context.

## Sources and Acknowledgments

This protocol is adapted conceptually from the BootLoops `referee-sim`
protocol, particularly its separation of correctness from framing, use of
fresh reviewer contexts, and emphasis on answering objections where readers
form their impressions.

See `reference/upstream.toml` for pinned upstream provenance.