# Public Diplomacy Simulation Lab (PDSL): Methods Note

**Version:** v1.1 (semantics, frozen) · v0.2.0 (architecture)  
**Author:** Frantz Damas  
**Date:** February 28, 2026  

---

## Abstract

The Public Diplomacy Simulation Lab (PDSL) is a deterministic, theory-constrained simulation framework designed for analytical demonstration and controlled scenario reasoning in public diplomacy contexts. PDSL does not perform empirical causal inference, forecasting, or predictive modeling. Instead, it operationalizes established theoretical constructs — algorithmic persuasion, identity alignment, and policy support under threat framing — within a governed analytical environment that emphasizes interpretive discipline and transparency of assumptions. Outputs are interpreted through a regime-based analytical framework rather than as standalone scores, ensuring that results remain analytically bounded and pedagogically legible.

This methods note documents the conceptual structure, assumptions, interpretive logic, and limitations of PDSL, providing a citable methodological reference that is independent of implementation details or operational mechanics. Model semantics are frozen at v1.1 and are stable for citation. Engine architecture was modularized in v0.2.0; this change is non-semantic and does not affect outputs, regimes, or interpretive logic.

---

## 1. Design Philosophy

PDSL is intentionally deterministic. Under identical analytical inputs, the framework produces identical outputs. This design choice prioritizes interpretability, reproducibility, and methodological clarity over stochastic realism or predictive power. PDSL is designed to support theoretical reasoning, sensitivity exploration, and structured interpretation — not empirical estimation, optimization, or policy automation.

Reproducibility is enforced by a hard gate (`/api/validate`) that verifies semantic integrity against a publicly committed canonical test vector on every deployment. This governance mechanism ensures that no architectural or infrastructural change can silently alter model behavior.

---

## 2. Version Discipline

PDSL separates two independent version tracks to prevent citation ambiguity:

| Track | Version | Scope |
|---|---|---|
| **Model semantics** | v1.1 (frozen) | All formulas, regime taxonomy, fatigue rule, saturation logic, and output behavior |
| **Engine architecture** | v0.2.0 | Internal modular layout — non-semantic, no effect on outputs |

Academic citations and policy references should anchor to **v1.1 semantics**. Architecture versioning is internal and not relevant to methodological reproducibility.

---

## 3. Core Outcome Channels

PDSL produces three analytically distinct outcome channels:

### Algorithmic Persuasion Risk (APR)
APR represents short-run susceptibility to attitudinal change under modeled conditions of exposure and framing pressure. It functions as a diagnostic signal rather than a proxy for policy support or approval.

### Identity Alignment Shift (IAS)
IAS captures slower, structural movement in identity alignment driven by exposure, identity salience, and time. It operates as a long-horizon contextual constraint rather than a short-run trigger.

### Policy Support via Threat Framing (PST)
PST represents policy support generated through threat framing under modeled conditions of exposure, identity salience, and time, subject to explicit diminishing returns under saturation. PST is interpreted only within the regime-based analytical framework described below.

---

## 4. Regime-Based Interpretation

PDSL does not interpret outcome values in isolation. Instead, outputs are read through a regime-based analytical framework that classifies system states into analytically meaningful regimes. These regimes govern interpretation by constraining:

- which mechanisms are analytically dominant,
- which narrative interpretations are permissible, and
- which policy-relevant cautions apply.

This regime-based approach prevents misinterpretation of outputs as linear effects, predictions, or direct policy recommendations. Six regimes (R0–R5) are defined and stable under v1.1 semantics.

---

## 5. Governance and Reviewability

PDSL adopts a governance-first posture designed to ensure internal coherence and interpretive consistency across analytical uses. Three mechanisms enforce this posture:

1. **Determinism** — identical inputs always produce identical outputs.
2. **Hard gate** — `/api/validate` verifies semantic integrity against the canonical test vector on every deployment.
3. **Public test vectors** — canonical inputs and expected outputs are committed at `docs/test-vectors/` and independently verifiable.

Outputs associated with PDSL v1.1 should be understood as deterministic, auditable "what-if" signals generated under explicitly stated assumptions.

---

## 6. Limits and Non-Claims

PDSL explicitly does not:

- perform causal inference or estimate treatment effects,
- forecast real-world behavior or policy outcomes,
- optimize decisions or recommend actions,
- model individual-level targeting or personalization, or
- operate as a decision-support or operational system.

All outputs are illustrative and analytical. Their validity is bounded by the theoretical assumptions encoded in the framework and by the regime-based interpretation that governs their use.

---

## Citation

Damas, F. (2026). *Public Diplomacy Simulation Lab (PDSL): Methods Note* (v1.1 semantics · v0.2.0 architecture). Deterministic simulation framework for analytical demonstration in public diplomacy. Public documentation release.
