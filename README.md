# SE Protocols: Research

Research protocols for Structural Explainability theory development,
source analysis, independent review, scientific acceptance, and external review.

## Scope

### source-audit

What does the existing system actually say?

Use when determining what current papers, specifications, formalizations,
registries, or repository artifacts explicitly define, require, omit,
or leave unresolved.

### theory-construction

What should the theory say?

Use when the scientific semantics, definitions, or structure are not yet
settled and a candidate theory must be proposed and tested.

Used during the 2026 October Theory Construction update.

### independent-review

Can another path break the proposed answer?

Use when an independent adversarial assessment is intended to provide
evidence about a proposed scientific result.

Used during the 2026 October Theory Construction update.

### theory-acceptance

Is the answer mature enough to become canonical?

Use after theory construction and independent review to decide whether a
scientific result is ready for canonical adoption.

### referee-sim

What will an informed outsider attack or misunderstand?

Use before circulating a paper, theory release, specification, or other
outward-facing scientific claim.

## Protocols

```text
protocols/
├── source-audit/
│   └── SKILL.md
├── theory-construction/
│   └── SKILL.md
├── independent-review/
│   └── SKILL.md
├── theory-acceptance/
│   └── SKILL.md
└── referee-sim/
    └── SKILL.md
```

Each protocol is a standalone instruction file intended for use by capable
human or AI-assisted research workflows.

The protocols govern research process and review.
They do not define Structural Explainability theory semantics.

## Workflow

A typical theory-development sequence is:

```text
source-audit
    ↓
theory-construction
    ↓
independent-review
    ↓
theory-acceptance
    ↓
canonical theory / formalization
    ↓
referee-sim before external circulation
```

Not every task requires every protocol.

For example,
a source audit may end with a documented finding and no new
theory construction,
while referee simulation applies primarily to
outward-facing artifacts.

## Adoption

Repositories that adopt these protocols declare that relationship in:

```text
.protocols/research.md
```

Example:

```markdown
# Research Protocols

<!--
WHY: This repository uses the Structural Explainability Research Protocols
for theory construction, independent review, and scientific acceptance.
-->

This repository uses the research protocols defined at:
<https://github.com/structural-explainability/se-protocols-research>

Research protocols govern research process and review.
They do not define theory semantics or alter this repository's authority model.
```

The adopting repository remains authoritative for its own theory,
specification, implementation, and evidence surfaces.

## Upstream Methodological Sources

Some protocols are informed by or adapted from external research-method
protocols.

Pinned upstream provenance is recorded in:

```text
reference/upstream.toml
```

External sources inform the research methodology.
They are not dependencies of Structural Explainability theory.

## Authority

The canonical protocol texts are the files under:

```text
protocols/*/SKILL.md
```

`reference/upstream.toml` records methodological provenance and attribution.

Generated or packaged copies, if added later for specific agent systems,
must be derived from the canonical protocol texts and must not become
independent sources of protocol authority.

## License

See [CC BY 4.0](./LICENSE).

## Citation

See [CITATION.cff](./CITATION.cff).

## References

See [BootLoops](https://github.com/BootLoops-ai/bootloops)
