# World Semantic Foundation

> **An authoritative, understandable, referenceable, machine-readable, executable, and integrable semantic foundation — bridging meaning, representation, execution, and application.**

The **World Semantic Foundation (WSF)** is a governed, versioned, authoritative semantic foundation from which downstream semantic systems — enterprise architecture, assessment models, knowledge graphs, AI agents, digital twins — may specialize, integrate, and extend without redefining foundational meaning.

Established by **CR-WSF-17 Rev.1** and governed by the **WSF Architectural Decision Records (ADRs)**, WSF bridges four normally separated concerns:

```
Meaning ──► Representation ──► Execution ──► Application
```

---

## 📚 The 8 Repositories

WSF is implemented as **8 specialized repositories**. Each repository has a clear role and they work together as a governed product foundation.

### 🏛️ Core Semantic Repositories

| Repository | Role | Status |
|---|---|---|
| [**wsf**](https://github.com/World-Semantic-Foundation/wsf) | Canonical semantic assets — authoritative concept definitions (Entity, Concept, Capability, etc.) | **Ready** |
| [**wsf-spec**](https://github.com/World-Semantic-Foundation/wsf-spec) | Normative semantic & conformance specifications | Scaffold |
| [**wsf-governance**](https://github.com/World-Semantic-Foundation/wsf-governance) | ADRs, CRs, governance, lifecycle, authority, investigation record | **Ready** |
| [**wsf-examples**](https://github.com/World-Semantic-Foundation/wsf-examples) | Reference applications (OTCHERE Inc, OTCHERE DC-01, Order Fulfillment Simulation) | **Ready** |

### ⚙️ Implementation Repositories

| Repository | Role | Status |
|---|---|---|
| [**wsf-software**](https://github.com/World-Semantic-Foundation/wsf-software) | Deployable WSF Semantic Engine (Store + Services + API) | Scaffold |
| [**wsf-connectors**](https://github.com/World-Semantic-Foundation/wsf-connectors) | Integration adapters for OpenDEA, EA platforms, KG platforms, AI agents | Scaffold |
| [**wsf-visuals**](https://github.com/World-Semantic-Foundation/wsf-visuals) | Reproducible visual semantic assets (Mermaid, PlantUML, SVG) | Scaffold |
| [**wsf-docs**](https://github.com/World-Semantic-Foundation/wsf-docs) | Conceptual & implementation documentation (12 Foundational Principles) | Partial |

---

## 🧭 How to Navigate the Org

### 1. New to WSF? Start here

1. Read the [**12 Foundational Principles**](https://github.com/World-Semantic-Foundation/wsf-docs/blob/main/conceptual/FOUNDATIONAL-PRINCIPLES.md)
2. Read the [**Top-Level README in `wsf-governance`**](https://github.com/World-Semantic-Foundation/wsf-governance) — explains the governance model
3. Browse the [**17+ ADRs**](https://github.com/World-Semantic-Foundation/wsf-governance/tree/main/ADR) — the architectural decisions
4. Browse the [**Tier 1 concepts**](https://github.com/World-Semantic-Foundation/wsf/tree/main/concepts) — the foundational semantics

### 2. Looking for something specific?

| If you want to understand... | Go to |
|---|---|
| **What WSF is and why** | [wsf-governance/README.md](https://github.com/World-Semantic-Foundation/wsf-governance) |
| **The 12 Foundational Principles** | [wsf-docs/conceptual/FOUNDATIONAL-PRINCIPLES.md](https://github.com/World-Semantic-Foundation/wsf-docs/blob/main/conceptual/FOUNDATIONAL-PRINCIPLES.md) |
| **How WSF is governed** | [wsf-governance/GOVERNANCE/](https://github.com/World-Semantic-Foundation/wsf-governance/tree/main/GOVERNANCE) |
| **What concepts are defined** | [wsf/concepts/](https://github.com/World-Semantic-Foundation/wsf/tree/main/concepts) |
| **The investigation history** | [wsf-governance/RESEARCH/INVESTIGATION-RECORD.md](https://github.com/World-Semantic-Foundation/wsf-governance/blob/main/RESEARCH/INVESTIGATION-RECORD.md) |
| **Worked examples** | [wsf-examples/](https://github.com/World-Semantic-Foundation/wsf-examples) |
| **The Software Engine** | [wsf-software/README.md](https://github.com/World-Semantic-Foundation/wsf-software) |
| **Integration architecture** | [wsf-connectors/README.md](https://github.com/World-Semantic-Foundation/wsf-connectors) |
| **Visualization conventions** | [wsf-visuals/README.md](https://github.com/World-Semantic-Foundation/wsf-visuals) |
| **How to write a new ADR** | [wsf-governance/templates/ADR-TEMPLATE.md](https://github.com/World-Semantic-Foundation/wsf-governance/blob/main/templates/ADR-TEMPLATE.md) |

### 3. Want to contribute?

WSF follows an **8-stage Change Control Lifecycle** with **6-stage Semantic Status** for every change. See:

- [Change Control Lifecycle](https://github.com/World-Semantic-Foundation/wsf-governance/blob/main/GOVERNANCE/CHANGE-CONTROL-LIFECYCLE.md) — Investigation → Finding → Synthesis → ADR → CR → Implementation → Validation → Release
- [Semantic Status Model](https://github.com/World-Semantic-Foundation/wsf-governance/blob/main/GOVERNANCE/SEMANTIC-STATUS-MODEL.md) — Candidate → Investigating → Proposed → Normative → Deprecated → Retired

---

## 🏛️ The 7-Capability Product Architecture

WSF provides **seven mutually reinforcing capabilities**:

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

## 🎯 What WSF Is — And What It Is Not

### WSF **IS**

- An **authoritative** semantic foundation (one meaning, one definition)
- **Understandable** — readable by humans and machines
- **Referenceable** — every concept has a stable identity
- **Machine-readable** — YAML, JSON-LD, RDF, OWL representations
- **Executable** — Semantic Engine + Connectors
- **Integrable** — with OpenDEA, EA platforms, KG platforms, AI agents
- **Visualizable** — reproducible semantic diagrams
- **Simulatable** — Digital Twin + Simulation patterns
- **Applicable** — to real entities, organizations, capabilities (e.g., OTCHERE Inc, Kwesi, Order Management)

### WSF **IS NOT**

- A flat vocabulary or terminology list
- An enterprise architecture metamodel (OpenDEA remains separate)
- An assessment model (Assessment-Models remains separate)
- A single ontology (WSF is a foundation for multiple ontologies)
- A specific technology (RDF, OWL, JSON-LD are implementation choices)
- A repository convention (architecture follows semantic responsibility)

---

## 🔍 The 13 Foundational Semantic Domains

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

## 🌐 Boundaries Preserved

WSF operates in a **federated ecosystem**:

- **WSF** — World semantics (this org)
- **OpenDEA** — Enterprise Architecture specialization (separate org)
- **Assessment-Models** — Maturity / Assessment governance (separate org)
- **Semantic Architecture / Ontology Architecture** — semantic & formal representation layers

These remain **independent lifecycle boundaries** with **governed semantic interfaces**.

---

## 🧬 Tier 1 Foundational Concepts (12/12 COMPLETE)

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

Plus **Capability** (Tier 3 specialized Disposition) as a worked example.

Browse them all: [github.com/World-Semantic-Foundation/wsf/tree/main/concepts](https://github.com/World-Semantic-Foundation/wsf/tree/main/concepts)

---

## 📜 Governance Model

WSF follows a strict governance discipline:

1. **No implementation without an ADR.** Every architectural decision is recorded.
2. **No ADR without investigation.** Every ADR traces to investigation.
3. **Investigation → Finding → Synthesis → ADR → CR → Implementation → Validation → Release.** The 8-stage lifecycle.
4. **Authority follows semantic responsibility** (not repository location).
5. **Concept Identity persists through compatible evolution** (per ADR-WSF-18).
6. **Meaning precedes representation** (per ADR-WSF-23 forthcoming).

---

## 📞 Canonical Example Convention

All WSF examples use:

- **Enterprise**: **OTCHERE Inc** (or OTCHERE)
- **Individual**: **Kwesi**
- **System**: **OTCHERE DC-01**

**ACME is prohibited.**

---

## 📅 Current State (2026-08-29)

| Component | Status |
|---|---|
| Phase 0 Baseline | FROZEN |
| ADRs | 22 (1 Accepted, 5 new Proposed in Phase 2) |
| Tier 1 concepts | 12/12 COMPLETE |
| Tier 3 example concepts | 1 (Capability) |
| Repositories live | 8 + .github profile |
| Reference examples | 3 (OTCHERE Inc, OTCHERE DC-01, Order Fulfillment Simulation) |
| Documentation | 12 Foundational Principles complete; rest scaffolded |
| Implementations | SCAFFOLD — awaiting ADR-WSF-24+ |

---

## 🔗 Quick Links

- **Top-Level Architecture**: [wsf-governance/README.md](https://github.com/World-Semantic-Foundation/wsf-governance)
- **Tier 1 Concepts**: [wsf/concepts/](https://github.com/World-Semantic-Foundation/wsf/tree/main/concepts)
- **All ADRs**: [wsf-governance/ADR/](https://github.com/World-Semantic-Foundation/wsf-governance/tree/main/ADR)
- **Examples**: [wsf-examples/](https://github.com/World-Semantic-Foundation/wsf-examples)
- **Principles**: [wsf-docs/conceptual/FOUNDATIONAL-PRINCIPLES.md](https://github.com/World-Semantic-Foundation/wsf-docs/blob/main/conceptual/FOUNDATIONAL-PRINCIPLES.md)

---

*WSF bridges meaning, representation, execution, and application — under governed, versioned, authoritative semantics.*
