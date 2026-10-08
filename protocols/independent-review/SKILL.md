---
name: independent-review
description: Obtain a genuinely independent adversarial assessment of a scientific claim, 
candidate definition, proof strategy, or theory decision. 
Use when agreement from another agent or reviewer is intended to provide 
evidential value rather than additional brainstorming.
---

# Independent Review

Use this protocol when a second review is intended to count as independent
evidence.

## Core Rule

Independence is a property of the reviewer's information path, 
not the reviewer's name or model.

Two agents are not independent merely because they are different agents.

## Procedure

### 1. Define the object under review

Provide the reviewer with the candidate claim, definition, proof, or theory
structure to test.

State:

- the exact question;
- settled background;
- permitted sources;
- forbidden assumptions;
- deferred issues.

### 2. Use a fresh review context

The reviewer should not inherit:

- the author's reasoning transcript;
- another reviewer's verdict;
- prior attempts to defend the candidate;
- hidden preferred conclusions.

Give only the information required to perform the review.

### 3. Prevent cross-reading

When multiple independent reviewers are used, do not show reviewer A's report
to reviewer B before B has completed its own analysis.

Sequential refinement is useful later, but it is not independent review.

### 4. Require adversarial testing

The reviewer must try to falsify the candidate.

Require, as appropriate:

- concrete counterexample;
- contradiction;
- boundary case;
- hidden assumption;
- circularity;
- algebraic failure;
- authority mismatch;
- unsupported generalization.

A review that only restates the candidate is not independent evidence.

### 5. Require explicit disposition

Use:

- ACCEPT
- ACCEPT WITH NARROWING
- REJECT
- INSUFFICIENT BASIS

The reviewer must state the reason for the disposition.

### 6. Record review provenance

For each review, record enough information to reconstruct the review path:

- reviewer or model class;
- date;
- candidate version or commit;
- supplied prompt or task;
- supplied source set;
- whether prior reviews were visible;
- resulting verdict.

Do not rely on memory of what the reviewer saw.

### 7. Compare only after independent completion

After independent reviews are complete, compare:

- convergent conclusions;
- independent counterexamples;
- conflicting assumptions;
- distinct narrowings;
- disagreements requiring another scientific question.

Agreement is strongest when the reviewers reach it through visibly different
reasoning paths.

### 8. Human inspection remains required

Independent agent agreement is not final scientific authority.

A human reviewer must inspect:

- the candidate;
- the counterexamples;
- the proposed narrowing;
- the final accepted definition.

## Failure Modes

- Same-context "independent" review.
- Reviewer B reading reviewer A before forming a judgment.
- Prompting reviewers with the desired answer.
- Counting stylistic agreement as semantic agreement.
- Treating model confidence as evidence.
- Omitting what sources the reviewer was allowed to inspect.
- Using two wrappers over the same inherited reasoning path.

## Completion Condition

An independent-review pass is complete when:

- the review object was fixed before review;
- the reviewer had a fresh information path;
- adversarial testing occurred;
- provenance is recorded;
- a disposition was returned;
- any disagreement is explicit rather than averaged away.

## Sources and Acknowledgments

This protocol is informed by BootLoops' independence-bookkeeping,
prove-protocol, and referee-simulation practices, 
especially their emphasis on lineage, fresh contexts, 
and adversarial review.

See `reference/upstream.toml` for pinned upstream provenance.