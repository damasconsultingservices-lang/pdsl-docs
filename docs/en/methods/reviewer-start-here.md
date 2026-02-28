# Reviewer Start Here

This page is a single-entry point for academic reviewers, policy analysts, and funding evaluators encountering PDSL for the first time.

---

## What is PDSL?

The **Public Diplomacy Simulation Lab (PDSL)** is a deterministic, theory-constrained simulation framework for controlled scenario reasoning in public diplomacy contexts. It is not a forecasting tool, causal inference engine, or machine-learning system. It is a governed analytical artifact designed for review, teaching, and structured scenario exploration.

---

## Start with the live demo

**[https://pdsl.damascis.com/demo](https://pdsl.damascis.com/demo)**

The demo runs against the production engine in real time. Try the default inputs, then modify them to observe regime transitions and sensitivity behavior. The governance proof block on the demo page allows you to verify semantic integrity directly via `/api/validate`.

---

## Key documents

| Document | Purpose |
|---|---|
| [Model Card](model-card.md) | Purpose, non-claims, inputs/outputs, governance summary |
| [Methods Note](methods-note.md) | Citable methods narrative — outcome channels, regimes, limits |
| [Review Protocol](review-protocol.md) | How to engage with PDSL outputs responsibly |
| [Governance](governance.md) | Disclosure boundary, versioning, semantic integrity enforcement |
| [Limitations](limitations.md) | Explicit constraints and non-claims |

---

## Canonical test vector

The v1.1 semantic baseline is publicly committed and independently verifiable.

| | |
|---|---|
| **Inputs** | `docs/test-vectors/canonical-input-v1.1.json` |
| **Expected outputs** | `docs/test-vectors/canonical-expected-v1.1.json` |
| **PST** | 0.636 |
| **Regime** | R2 |
| **Fatigue** | false |
| **Live verification** | `POST https://pdsl.damascis.com/api/validate` → `ok: true` |

[View test vectors on GitHub](https://github.com/damasconsultingservices-lang/pdsl/tree/main/docs/test-vectors)

---

## Version summary

| Track | Version | Meaning |
|---|---|---|
| **Model semantics** | v1.1 (frozen) | Stable for citation — formulas, regimes, fatigue rule unchanged |
| **Engine architecture** | v0.2.0 | Internal modularization only — non-semantic |

For citation, anchor to **v1.1 semantics**.

---

## Citation

Damas, F. (2026). *Public Diplomacy Simulation Lab (PDSL)* (v1.1 semantics · v0.2.0 architecture). Deterministic simulation framework for analytical demonstration in public diplomacy. [https://pdsl.damascis.com/demo](https://pdsl.damascis.com/demo)
