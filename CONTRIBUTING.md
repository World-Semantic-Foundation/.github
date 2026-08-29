# Contributing to World Semantic Foundation

> **WSF follows a strict governance discipline. All contributions go through the ADR → CR process.**

Thank you for your interest in contributing to the World Semantic Foundation. WSF is a **governed, versioned, authoritative semantic foundation** — meaning contributions are carefully managed to preserve semantic integrity, traceability, and conformance.

---

## The Contribution Process

WSF follows an **8-stage Change Control Lifecycle**:

```
Investigation → Finding → Synthesis → ADR → CR → Implementation → Validation → Release
```

Every change goes through all 8 stages. There are **no shortcuts**.

### 1. Investigation

Before proposing any change, conduct an investigation:

- Read the existing ADRs that govern the area
- Read the Investigation Record: [RESEARCH/INVESTIGATION-RECORD.md](https://github.com/World-Semantic-Foundation/wsf-governance/blob/main/RESEARCH/INVESTIGATION-RECORD.md)
- Identify whether the change is architectural (ADR), implementational (CR), or both
- Use the [ADR Template](https://github.com/World-Semantic-Foundation/wsf-governance/blob/main/templates/ADR-TEMPLATE.md) and [CR Template](https://github.com/World-Semantic-Foundation/wsf-governance/blob/main/templates/CR-TEMPLATE.md) to draft

### 2. Finding

Lift findings into `01_findings/` style numbered records (F-NNN-slug.md format).

### 3. Synthesis

Synthesize findings into a coherent proposal. Identify:
- What is being changed
- Why it is being changed
- What alternatives were considered
- What consequences are accepted
- What is explicitly NOT being decided

### 4. ADR (Architectural Decision Record)

If the change is architectural (governs meaning, structure, or process):
- Create `ADR-WSF-NN-<decision>.md` in `wsf-governance/ADR/`
- Use the ADR Template
- Status begins as `Proposed`
- Submit via PR

### 5. CR (Change Request)

If the change is implementational:
- Create `CR-WSF-NN-<change>.md` in `wsf-governance/CR/`
- Reference the ADR(s) it implements
- Use the CR Template
- Submit via PR

### 6. Implementation

After ADR/CR approval, implementation proceeds through normal Git workflow:
- Branch per task (`feature/<description>`, `fix/<description>`, etc.)
- Atomic commits
- Tests pass before merge
- Cross-references added

### 7. Validation

After implementation, validate:
- Semantic correctness
- Cross-reference integrity
- Conformance to specifications
- Documentation completeness

### 8. Release

Release through governance:
- Update version numbers per ADR-WSF-16
- Update CHANGELOG (per repo)
- Mark ADRs as Accepted
- Update top-level README where appropriate

---

## The 6-Stage Semantic Status Model

Every semantic artifact moves through:

```
Candidate → Investigating → Proposed → Normative → Deprecated → Retired
```

Status changes happen through ADRs, not through direct edits.

---

## The 12 Foundational Principles

All contributions must respect the [12 Foundational Principles](https://github.com/World-Semantic-Foundation/wsf-docs/blob/main/conceptual/FOUNDATIONAL-PRINCIPLES.md):

1. **Semantic Primacy** — Meaning precedes representation
2. **Minimal Foundation** — Smallest sufficiently expressive foundation
3. **Explicit Specialization** — Domain concepts specialize, not redefine
4. **Versioned Evolution** — Changes are governed
5. **Authoritative Provenance** — Sources are tracked
6. **Governance First** — Architecture precedes implementation
7. **Layered Realization** — Multiple levels, distinct concerns
8. **Traceable Rationale** — Decisions have documented reasoning
9. **Constrained Extensibility** — Extensions are governed
10. **Verifiable Conformance** — Claims are demonstrable
11. **Identity by Meaning** — Identity persists through change
12. **Investigation-Driven** — Decisions follow research

---

## The Canonical Example Convention

All examples in WSF documentation MUST use:

- **Enterprise**: **OTCHERE Inc** (or OTCHERE)
- **Individual**: **Kwesi**
- **System**: **OTCHERE DC-01**

**ACME is prohibited** in all WSF artifacts.

---

## Repository Etiquette

When contributing to a specific repository:

- **wsf**: New foundational concepts, refinements to existing concepts
- **wsf-spec**: Normative specifications, conformance tests
- **wsf-governance**: ADRs, CRs, governance documents, investigation records
- **wsf-examples**: Reference applications, digital twin examples, simulation examples
- **wsf-software**: Engine implementation, services, APIs
- **wsf-connectors**: Integration adapters
- **wsf-visuals**: Visual asset sources (Mermaid, PlantUML, etc.)
- **wsf-docs**: Conceptual documentation, tutorials

Always **cross-reference** related concepts/ADRs using stable links.

---

## Style Guide

- **Markdown** for prose
- **YAML** for structured data (preferred for semantic assets)
- **Mermaid** for diagrams (preferred source format)
- **English** throughout
- **Examples**: Use OTCHERE Inc / Kwesi / OTCHERE DC-01
- **Versions**: Follow semver for semantic content per ADR-WSF-16
- **Dates**: ISO 8601 format

---

## Questions?

Open an issue or start a discussion. Complex architectural questions should become ADRs; implementation questions should reference ADRs.

---

*By contributing to WSF, you agree to follow its governance model and principles.*
