# PDSL Model Card (Public)

## 1. Model Name
**Public Diplomacy Simulation Lab (PDSL)**  
Public documentation release

## 2. Version / Release Anchor

| Track | Version | Status |
|---|---|---|
| **Model semantics** | v1.1 | Frozen — all formulas, regime taxonomy, fatigue rule, and compute() logic are stable and citable |
| **Engine architecture** | v0.2.0 | Modularized internal layout — no change to outputs or analytical behavior |

> **For citation purposes, reference v1.1 semantics.** Architecture versioning is internal and non-semantic.

---

## 3. Summary
The **Public Diplomacy Simulation Lab (PDSL)** is a **deterministic, theory-constrained simulation framework** designed for **analytical demonstration and controlled scenario reasoning** in public diplomacy and digitally mediated influence contexts.

PDSL is governance-first by design. It emphasizes **interpretive discipline, transparency of assumptions, and explicit non-claims**, rather than prediction, optimization, or empirical inference.

---

## 4. What PDSL *Is*
- A **deterministic simulation framework** that maps structured analytical inputs to consistent, interpretable outputs
- A **controlled environment** for testing regime-defined narrative dynamics and sensitivity behavior
- A **reviewable demonstration artifact** intended for academic, policy, and educational audiences

---

## 5. What PDSL *Is Not*
PDSL is explicitly **not**:
- Empirical causal inference
- A predictive model of real-world publics
- A substitute for validated surveys, experiments, or field studies
- A machine-learning or black-box system

Outputs should not be interpreted as measurements of population attitudes or behavioral effects.

---

## 6. Architecture Overview (v0.2.0)

PDSL v0.2.0 adopts a **modular internal architecture** organized into discrete library components. This is an internal structural change only — it does not alter model semantics, output behavior, or the governance posture of the framework.

The public API surface remains unchanged:
- `POST /api/simulate` — single-scenario simulation
- `POST /api/scenario` — multi-phase path simulation
- `POST /api/sensitivity` — ASPE slope analysis
- `POST /api/validate` — **hard gate**: verifies semantic integrity against canonical test vector

The `/api/validate` hard gate enforces that v1.1 semantics are intact on every deployment. Canonical verification inputs and expected outputs are publicly committed at:
[`docs/test-vectors/`](https://github.com/damasconsultingservices-lang/pdsl/tree/main/docs/test-vectors)

---

## 7. Methods (Conceptual Overview)
PDSL implements a **deterministic, theory-constrained simulation design** for controlled scenario reasoning. Rather than estimating causal effects or forecasting outcomes, it operationalizes a **regime-based interpretive framework** that translates structured analytical inputs into three analytically distinct outcome channels:

- **Algorithmic Persuasion Risk (APR)**
- **Identity Alignment Shift (IAS)**
- **Policy Support via Threat Framing (PST)**

The framework is designed so that **interpretation is governed by regimes**, not by raw numerical values or analyst discretion.

---

## 8. Conceptual Inputs (High-Level)
Public documentation describes inputs **abstractly**. These include representations of:
- Exposure or distribution pressure
- Framing and narrative intensity (including saturation effects)
- Identity salience
- AI / media literacy context
- Time or iteration horizon

This release does not disclose parameter thresholds, equations, or engine-specific mechanics.

---

## 9. Outputs (Governed Outcome Channels)

### APR — Algorithmic Persuasion Risk
APR captures **short-run susceptibility to attitudinal change** under modeled exposure and framing pressure.
APR functions as a **diagnostic risk signal**, not as a proxy for policy support or approval.

### IAS — Identity Alignment Shift
IAS captures **slower, structural movement in identity alignment** driven by exposure, identity salience, and time.
IAS acts as a **long-horizon constraint**, not as a trigger for short-run interpretation.

### PST — Policy Support via Threat Framing
PST represents **policy support generated through threat framing**, subject to **explicit diminishing returns under saturation**.
PST is interpreted **only through the regime-based framework**, never as a standalone score.

---

## 10. Regime-Based Interpretation
PDSL does not interpret outputs independently. Instead, outputs are read through **named analytical regimes** that:

- Constrain appropriate policy interpretation
- Enable modular and comparable scenario reasoning
- Prevent over-reading of marginal score changes

The same output value may imply escalation, plateau, or diminishing returns depending on regime context.

---

## 11. Interpretability Guardrails
- APR, IAS, and PST are **analytical constructs**, not empirical measurements
- Outputs are **comparative signals**, not predictions
- Interpretation requires
