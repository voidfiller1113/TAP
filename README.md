# TAP: The Architect's Protocol

![Version: 2.0.0](https://img.shields.io/badge/Version-2.0.0-green?style=flat-square)
![Status: Normative Standard](https://img.shields.io/badge/Status-Normative%20Standard-black?style=flat-square)
![Role: L2 Structure](https://img.shields.io/badge/Role-L2%20Structure-blue?style=flat-square)
![Requirement: Deterministic Actor](https://img.shields.io/badge/Requirement-Deterministic%20Actor-red?style=flat-square)
![Scope: Pure Abstract](https://img.shields.io/badge/Scope-Pure%20Abstract-purple?style=flat-square)
![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey?style=flat-square)

**Version:** 2.0.0 (Pure Abstract Core)
**Status:** Normative Standard / Immutable
**Publisher:** void-filler

---

## Overview

TAP is a formal specification for bridging the structural void between Concept (L3) and Implementation (L1). It defines the **Structure (L2)** through which all intent must pass to become execution.

This repository contains the **Core Specification**. It defines the Axioms, Interfaces, and Protocol Lifecycle that constitute the invariant laws of the system.

## Sovereignty Matrix

To ensure clear separation of concerns, authority is divided between the Protocol (this specification) and the Domain Architect (the implementer).

| Domain | TAP Authority (Normative) | Domain Architect Authority (Implementation) |
|:---|:---|:---|
| **Axioms** | Defines Invariants | **Must Satisfy** Invariants |
| **Logic** | Requires Formalization | Writes the Formal Logic |
| **Verification** | Requires Proof of Determinism | Selects Proof Method (e.g., Test Suites, Formal Proofs) |
| **Execution** | Requires Deterministic Actor | Selects Actor (e.g., AI Agents, Code) |

## Implementation Policy

### The Structural Mandate (AI/Actor Requirement)
Conformance to **Axiom 4 (Interpretation Independence)** necessitates the use of Deterministic Actors.

Unassisted human execution is inherently probabilistic, possesses opaque internal states, and cannot guarantee interpretation independence. Therefore, **human-only implementations are Non-Compliant by definition.** TAP does not recognize systems executed solely by biological operators.

### The Delegation of Implementation ("Marunage")
This repository provides only the Normative Specification (The "What" and "Why").

**Implementation guidelines, tutorials, specific tooling, and prompts are deliberately excluded.**

Binding this protocol to specific technologies (such as Python or specific Large Language Models) would violate its timeless nature. The translation of this abstract specification into concrete tools is the **sole responsibility and sovereignty of the Domain Architect**.

## Documentation

| Document | Content |
|----------|---------|
| [00_Overview](./spec/00_Overview.md) | Four Axioms + Deterministic Actor Definition |
| [01_Interface](./spec/01_Interface.md) | ITap Contract + Invariant Constraints |
| [02_Protocol](./spec/02_Protocol.md) | 5-Phase Lifecycle |

## License

This work is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0).
