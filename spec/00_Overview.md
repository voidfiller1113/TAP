# TAP Specification: Overview

**Document ID:** TAP-SPEC-00
**Version:** 2.0.0 (Pure Abstract Core)
**Status:** Normative / Immutable
**Publisher:** void-filler

---

## 1. Purpose

The Architect's Protocol (TAP) is a formal specification for bridging the structural void between Abstract Concept (L3) and Concrete Implementation (L1). This document defines the foundational Axioms and Actor definitions that govern the protocol. These definitions are invariant and not subject to modification.

---

## 2. The Four Axioms

Any system claiming conformance to TAP must satisfy the following four axioms without exception.

### 2.1 Axiom 1: The Axiom of Separation
> **Concept (L3) and Implementation (L1) must never connect directly.**

All signals transmitting intent from L3 to L1 must pass through a defined Structure (L2). Direct coupling between intent and execution creates implicit dependencies and prevents structural reasoning.

### 2.2 Axiom 2: The Axiom of Explicit State
> **All structural voids must be filled by explicit, documented Proxies.**

The gap between layers must be bridged by formal architectural components (Proxies). Reliance on tacit knowledge, heroic individual effort, or undocumented workflows to bridge layers is a violation of this axiom.

### 2.3 Axiom 3: The Axiom of Finite Sovereignty
> **Every architectural component must have explicitly defined boundaries and failure modes.**

Infinite authority or undefined behavior is prohibited. Every Proxy must declare its scope, scale, and authority limits, and explicitly define its behavior when those limits are exceeded.

### 2.4 Axiom 4: The Axiom of Interpretation Independence
> **Transformation logic must be formally encoded such that its execution path is predetermined by Input and Context, requiring zero stochastic interpretation.**

The logic defining L2 transformations must be rigorous enough that the output is mathematically or logically derivable solely from the declared state. If the execution requires a probabilistic guess or operator intuition, it violates this axiom.

---

## 3. Actor Definition

To satisfy Axiom 4, the executing entity of the protocol is strictly defined.

### 3.1 Deterministic Actor
A **Deterministic Actor** is the only authorized executor of TAP Proxies. It is defined as an entity satisfying the following three conditions:

1.  **Governed by Rules:** Its execution is strictly governed by explicit, pre-inspectable Rules.
2.  **Transparent State:** Its internal state during transformation is either null or transparent to external verification.
3.  **Invariant Output:** It produces invariant output for any given pair of `(Input, Context)`.

**Note:** Unassisted human operators are inherently probabilistic and possess opaque internal states. Therefore, humans do not qualify as Deterministic Actors.
