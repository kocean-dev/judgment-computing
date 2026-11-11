# Judgment Computing: Conceptual Glossary & Taxonomy

> **Version 2.0.0** — November 2026  
> **Author**: YL Khim  
> **DOI**: [10.5281/zenodo.23388471](https://doi.org/10.5281/zenodo.23388471)  
> **License**: [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)

---

## Overview

This glossary defines the foundational concepts, principles, and architectural terms introduced in **Judgment Computing** (*The Final Question of AI Computing*). It establishes an open, vendor-neutral taxonomy for systems that operate beyond conversational intelligence, focusing on authority, constitutional governance, execution verification, and human-sovereign judgment.

---

## Core Taxonomy

### 1. Judgment Computing
The theoretical and architectural paradigm of computing that emerges after Command, Application, Workflow, Work, Intent, Context, and Trust Computing. It addresses situations where multiple valid principles or rules conflict, complete information is unavailable, and decisions require value prioritization and moral or legal accountability.

### 2. Judgment-Aware Computing
The practical systems model of Judgment Computing. Rather than attempting to compute or simulate subjective values autonomously, a **Judgment-Aware System** is architecturally designed to:
1. Distinguish between deterministic execution domains and value-laden judgment domains.
2. Identify rule and value collisions transparently.
3. Quantify risk, surface precedent, and present options.
4. Step back and yield final decision-making power to human authority whenever boundaries or constitutional thresholds are encountered.

### 3. Intent Contract
An explicit, mutually negotiated, and cryptographically verifiable operational agreement between a human and an autonomous system. It formalizes a user’s incomplete natural-language intent into an enforceable specification covering:
- Permitted objectives and out-of-scope boundaries
- Authorized data scopes and credential delegation
- Mandatory validation checkpoints (synchronous approval gates)
- Pre-approved rollback and compensation paths

### 4. Intent Discovery
The initial interactive phase in which a system identifies the ambiguities, unstated assumptions, missing constraints, and implicit risks in a user's initial prompt before initiating execution. A mature system prioritizes **discovery and negotiation over blind execution**.

### 5. Capability vs. Authority
A foundational distinction asserting that:
> *Intelligence is capability; it is never authority.*

A system may possess the computational power, tool interfaces, and API access to perform an action (Capability), but it is never permitted to act unless an explicit, legitimate mandate has been delegated through an Intent Contract (Authority).

### 6. Physics Over Policy
The architectural security principle stating that prohibited actions must be rendered **structurally and physically impossible** by the environment's boundary layer, rather than merely forbidden through prompt instructions, policies, or post-hoc auditing. If a path is unauthorized, no execution channel exists.

### 7. Boundary (Behavior Layer)
The rule-based execution layer that defines how components, data, and work units interact. The Boundary separates **what a component can do** (Capability) from **how and under what conditions it behaves** (Behavior).
- In user experience, boundaries decouple logical connection from screen coordinates, allowing flexible layout, styling, and AI-assisted ergonomic arrangement.
- In security, boundaries act as unbreachable structural containment walls (*Physics Over Policy*).

### 8. Preserve the Constitution, Replace the Engines
The architectural maxim stating that while underlying AI models and execution engines are volatile and frequently deprecated, the normative criteria, value priorities, and inviolable boundaries must reside in an independent, persistent **Constitutional Layer** outside the models.
- Systems change engines as easily as users change web browsers.
- The Constitution remains steady, auditable, and sovereign.

### 9. Constitution (Operational Framework)
The supreme normative hierarchy governing all policies, contracts, delegations, and runtime recovery strategies within a system or organization:
$$\text{Human Sovereignty} \to \text{Values} \to \text{Principles} \to \text{Constitution} \to \text{Governance \& Policy} \to \text{Execution}$$
- Specialized constitutions may exist for different domains (medical, financial, personal), but all share the inviolable premise of **Human Final Authority**.
- Constitutional amendments require physically isolated, multi-party authorized procedures, distinct from day-to-day policy overrides.

### 10. Memory of Work (Transformation Memory)
A persistence model that records not merely static file snapshots, window placements, or conversational transcripts, but the **trajectory of work transformation**:
$$\text{Raw Execution Log} \longrightarrow \text{Pattern Discovery} \longrightarrow \text{Work Knowledge}$$
It preserves *why* decisions were made, how drafts evolved, and how past precedents resolved conflicts.

### 11. Work Unit
The fundamental primitive of human computing activity that replaces the application window. A Work Unit binds components, intent, contextual memory, and boundaries around a coherent human objective (e.g., *Customer Incident Response*, *Seminar Preparation*). Work units can be recursively nested within larger work units.

### 12. Justified Override (Explainable Exception & Precedent)
A structured mechanism allowing an authorized human to temporarily bypass a standard rule in emergency or high-stakes situations (e.g., an ER physician accessing records without prior patient consent).
- The override does **not** silently alter the Constitution or rules.
- It records who broke the rule, why it was justified, which higher value was preserved, and what risk was assumed, crystallizing into a transparent **Precedent (판례)** for future audit and review.

### 13. Progressive Runtime Activation (Levels 0 to 4)
An efficiency and reliability principle: *Activate the minimum complexity required for success*.
- **Level 0 (Command)**: Simple deterministic tool invocation (open, print, save).
- **Level 1 (Composition)**: Ad-hoc component combination on a work surface.
- **Level 2 (Boundary Execution)**: Conditional logic and data transformation rules.
- **Level 3 (Knowledge & Governance)**: Contract validation, policy checks, approval gates.
- **Level 4 (Verification & Recovery)**: Formal proof verification, certified manifest enforcement, and multi-tier autonomous recovery.

---

## Citation

To cite this glossary:

```bibtex
@misc{khim2026judgmentglossary,
  author       = {Khim, Y. L.},
  title        = {Judgment Computing: Conceptual Glossary and Taxonomy},
  year         = {2026},
  month        = nov,
  publisher    = {Zenodo},
  version      = {2.0.0},
  doi          = {10.5281/zenodo.23388471},
  url          = {https://doi.org/10.5281/zenodo.23388471}
}
```
