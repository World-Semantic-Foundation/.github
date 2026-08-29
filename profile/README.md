# World Semantic Foundation

> **An authoritative, governed semantic foundation bridging meaning, representation, execution, and application.**

The **World Semantic Foundation (WSF)** provides a governed, versioned, authoritative semantic foundation from which downstream semantic systems — enterprise architecture, assessment models, knowledge graphs, AI agents, and digital twins — specialize, integrate, and extend without redefining foundational meaning.

The architecture bridges four normally separated concerns:

```
Meaning ──► Representation ──► Execution ──► Application
```

---

## The 8 Repositories

WSF is implemented as **8 specialized repositories**. Each repository has a clear role and they work together as a governed product foundation.

### Core Semantic Repositories

| Repository | Role | Status |
|---|---|---|
| [**wsf**](https://github.com/World-Semantic-Foundation/wsf) | Canonical semantic assets — authoritative concept definitions (Entity, Concept, Capability, Relationship, Event, State, Disposition, Proposition, Assertion, Identity, Context, Time, Space) | **Baseline** |
| [**wsf-spec**](https://github.com/World-Semantic-Foundation/wsf-spec) | Normative semantic & conformance specifications | Scaffold |
| [**wsf-governance**](https://github.com/World-Semantic-Foundation/wsf-governance) | Architectural decisions, change requests, governance, lifecycle, authority, investigation record | **Baseline** |
| [**wsf-examples**](https://github.com/World-Semantic-Foundation/wsf-examples) | Reference applications (OTCHERE Inc, OTCHERE DC-01, Order Fulfillment Simulation) | **Baseline** |

### Implementation Repositories

| Repository | Role | Status |
|---|---|---|
| [**wsf-software**](https://github.com/World-Semantic-Foundation/wsf-software) | WSF Semantic Engine (Semantic Store + Services + API layer) | Scaffold |
| [**wsf-connectors**](https://github.com/World-Semantic-Foundation/wsf-connectors) | Integration adapters for OpenDEA, EA platforms, KG platforms, AI agents | Scaffold |
| [**wsf-visuals**](https://github.com/World-Semantic-Foundation/wsf-visuals) | Reproducible visual semantic assets (Mermaid, PlantUML, SVG) | Scaffold |
| [**wsf-docs**](https://github.com/World-Semantic-Foundation/wsf-docs) | Conceptual & implementation documentation (12 Foundational Principles) | Partial |

---

## How to Navigate the Org

### For Newcomers

1. The [**12 Foundational Principles**](https://github.com/World-Semantic-Foundation/wsf-docs/blob/main/conceptual/FOUNDATIONAL-PRINCIPLES.md)
2. The [**Top-Level README in `wsf-governance`**](https://github.com/World-Semantic-Foundation/wsf-governance)
3. The [**17+ Architectural Decision Records**](https://github.com/World-Semantic-Foundation/wsf-governance/tree/main/ADR)
4. The [**Tier 1 concepts**](https://github.com/World-Semantic-Foundation/wsf/tree/main/concepts)

### For Specific Lookups

| To understand... | See |
|---|---|
| What WSF is and why | [wsf-governance/README.md](https://github.com/World-Semantic-Foundation/wsf-governance) |
| The 12 Foundational Principles | [wsf-docs/conceptual/FOUNDATIONAL-PRINCIPLES.md](https://github.com/World-Semantic-Foundation/wsf-docs/blob/main/conceptual/FOUNDATIONAL-PRINCIPLES.md) |
| How WSF is governed | [wsf-governance/GOVERNANCE/](https://github.com/World-Semantic-Foundation/wsf-governance/tree/main/GOVERNANCE) |
| What concepts are defined | [wsf/concepts/](https://github.com/World-Semantic-Foundation/wsf/tree/main/concepts) |
| The investigation history | [wsf-governance/RESEARCH/INVESTIGATION-RECORD.md](https://github.com/World-Semantic-Foundation/wsf-governance/blob/main/RESEARCH/INVESTIGATION-RECORD.md) |
| Worked examples | [wsf-examples/](https://github.com/World-Semantic-Foundation/wsf-examples) |
| The Semantic Engine architecture | [wsf-software/README.md](https://github.com/World-Semantic-Foundation/wsf-software) |
| Integration architecture | [wsf-connectors/README.md](https://github.com/World-Semantic-Foundation/wsf-connectors) |
| Visualization conventions | [wsf-visuals/README.md](https://github.com/World-Semantic-Foundation/wsf-visuals) |
| How to author a new ADR | [wsf-governance/templates/ADR-TEMPLATE.md](https://github.com/World-Semantic-Foundation/wsf-governance/blob/main/templates/ADR-TEMPLATE.md) |

---

## The 7-Capability Product Architecture

The WSF Product Foundation provides seven mutually reinforcing capabilities:

```
                          WSF
                           │
        ┌──────────────────┼──────────────────┐
        ▼                  ▼                  ▼
   SEMANTIC          KNOWLEDGE             SEMANTIC
   FOUNDATION         ASSETS               ENGINE
        │                  │                  │
        ▼                  ▼                  ▼
   INTEGRATION ──► VISUALIZATION ──► REALIZATION
                          │
                  supported by
                          │
                       GOVERNANCE
```

| # | Capability | Repository |
|---|---|---|
| 1 | **Semantic Foundation** | `wsf` |
| 2 | **Knowledge Assets** | `wsf-docs` + `wsf-spec` |
| 3 | **Semantic Engine** | `wsf-software` |
| 4 | **Integration** | `wsf-connectors` |
| 5 | **Visualization** | `wsf-visuals` |
| 6 | **Realization** | `wsf-examples` |
| 7 | **Governance** (wraps all 6) | `wsf-governance` |

---

## What WSF Provides

The architecture establishes an authoritative semantic layer that:

- **Establishes meaning** through 12 Tier 1 foundational concepts (Entity, Concept, Relationship, Event, State, Disposition, Proposition, Assertion, Identity, Context, Time, Space)
- **Enables specialization** through governed inheritance rules
- **Supports assertion** of facts with full provenance, evidence, and trust evaluation
- **Maintains identity** across representation, context, version, and lifecycle changes
- **Validates conformance** through semantic constraint checking
- **Versions evolution** while preserving semantic lineage

## What WSF Is Not

- A flat vocabulary or terminology list
- An enterprise architecture metamodel (OpenDEA remains separate)
- An assessment model (Assessment-Models remains separate)
- A specific ontology technology (RDF/OWL/JSON-LD are implementation choices)
- A repository convention (architecture follows semantic responsibility)

---

## The 13 Foundational Semantic Domains

WSF recognizes the following foundational semantic domains:

| Domain | Examples |
|---|---|
| **Existence** | Entity, Concept, Identity |
| **Occurrence** | Event |
| **Condition** | State, Disposition |
| **Relation** | Relationship, Specialization |
| **Identity** | Identity, Identifier, Reference |
| **Semantics** | Definition, Specification, Context |
| **Proposition** | Proposition, Assertion |
| **Qualification** | Context, Validation |
| **Temporality** | Time, Event |
| **Spatiality** | Space, Position, Region |
| **Epistemics** | Provenance, Evidence, Trust |

---

## Boundaries Preserved

WSF operates in a federated ecosystem with explicit boundary preservation:

- **WSF** — World semantics
- **OpenDEA** — Enterprise Architecture specialization (separate org)
- **Assessment-Models** — Maturity / Assessment governance (separate org)
- **Semantic Architecture / Ontology Architecture** — semantic & formal representation layers

Each maintains independent lifecycle boundaries with governed semantic interfaces.

---

## Tier 1 Foundational Concepts (12/12 Baseline)

| # | Concept | Tier | Domain |
|---|---|---|---|
| 1 | **Entity** | 1 | Existence |
| 2 | **Concept** | 1 | Existence / Semantics |
| 3 | **Relationship** | 1 | Relation |
| 4 | **Event** | 1 | Occurrence / Temporality |
| 5 | **State** | 1 | Condition |
| 6 | **Disposition** | 1 | Condition (Capacity, Ability, Capability) |
| 7 | **Proposition** | 1 | Proposition |
| 8 | **Assertion** | 1 | Proposition (attributed, evidenced) |
| 9 | **Identity** | 1 | Identity |
| 10 | **Context** | 1 | Qualification |
| 11 | **Time** | 1 | Temporality |
| 12 | **Space** | 1 | Spatiality |

**Capability** (Tier 3 specialized Disposition) is included as a worked example.

Browse them: [github.com/World-Semantic-Foundation/wsf/tree/main/concepts](https://github.com/World-Semantic-Foundation/wsf/tree/main/concepts)

---

## Governance Model

The architecture operates under these governance disciplines:

1. **Investigation before implementation.** Every architectural decision traces to documented investigation.
2. **Decisions are explicit.** The architectural decision record (ADR) is the authoritative architectural statement.
3. **Implementation is traceable.** Change requests implement ADRs with explicit scope.
4. **Lifecycle is governed.** Semantic artifacts move through defined status states.
5. **Authority follows semantic responsibility.** Not repository location.
6. **Identity persists through compatible evolution.** Meaning-based identifiers survive representation, context, and version changes.
7. **Meaning precedes representation.** Semantic authority is independent of format.

---

## Canonical Example Convention

All WSF documentation uses:

- **Enterprise**: **OTCHERE Inc** (or OTCHERE)
- **Individual**: **Kwesi**
- **System**: **OTCHERE DC-01**

Other enterprise names are not used in WSF artifacts.

---

## Current State

| Component | Status |
|---|---|
| Foundational semantic baseline | Final |
| Architectural decision records | 22 records (1 final, 21 baseline) |
| Tier 1 concepts | 12/12 final |
| Tier 3 example concepts | 1 (Capability) |
| Repositories live | 8 |
| Reference examples | 3 (OTCHERE Inc, OTCHERE DC-01, Order Fulfillment Simulation) |
| Documentation | 12 Foundational Principles complete; remaining documentation scaffolded |
| Implementations | Scaffold; specifications provided by subsequent architectural decisions |

---

## Quick Links

- **Top-Level Architecture**: [wsf-governance/README.md](https://github.com/World-Semantic-Foundation/wsf-governance)
- **Tier 1 Concepts**: [wsf/concepts/](https://github.com/World-Semantic-Foundation/wsf/tree/main/concepts)
- **All Architectural Decisions**: [wsf-governance/ADR/](https://github.com/World-Semantic-Foundation/wsf-governance/tree/main/ADR)
- **Examples**: [wsf-examples/](https://github.com/World-Semantic-Foundation/wsf-examples)
- **Principles**: [wsf-docs/conceptual/FOUNDATIONAL-PRINCIPLES.md](https://github.com/World-Semantic-Foundation/wsf-docs/blob/main/conceptual/FOUNDATIONAL-PRINCIPLES.md)

---

*WSF bridges meaning, representation, execution, and application — under governed, versioned, authoritative semantics.*
