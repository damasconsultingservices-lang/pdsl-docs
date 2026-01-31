# PDSL Model Card (Public)

## 1. Model Name
**Public Diplomacy Simulation Lab (PDSL)**  
Public documentation release

## 2. Version / Release Anchor
**v0.1.1-review-ready**

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

## 6. Methods (Conceptual Overview)
PDSL implements a **deterministic, theory-constrained simulation design** for controlled scenario reasoning. Rather than estimating causal effects or forecasting outcomes, it operationalizes a **regime-based interpretive framework** that translates structured analytical inputs into three analytically distinct outcome channels:

- **Algorithmic Persuasion Risk (APR)**  
- **Identity Alignment Shift (IAS)**  
- **Policy Support via Threat Framing (PST)**  

The framework is designed so that **interpretation is governed by regimes**, not by raw numerical values or analyst discretion.

---

## 7. Conceptual Inputs (High-Level)
Public documentation describes inputs **abstractly**. These include representations of:
- Exposure or distribution pressure  
- Framing and narrative intensity (including saturation effects)  
- Identity salience  
- AI / media literacy context  
- Time or iteration horizon  

This release does not disclose parameter thresholds, equations, or engine-specific mechanics.

---

## 8. Outputs (Governed Outcome Channels)

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

## 9. Regime-Based Interpretation
PDSL does not interpret outputs independently. Instead, outputs are read through **named analytical regimes** that:

- Constrain appropriate policy interpretation  
- Enable modular and comparable scenario reasoning  
- Prevent over-reading of marginal score changes  

The same output value may imply escalation, plateau, or diminishing returns depending on regime context.

---

## 10. Interpretability Guardrails
- APR, IAS, and PST are **analytical constructs**, not empirical measurements  
- Outputs are **comparative signals**, not predictions  
- Interpretation requires regime context and documented assumptions  

---

## 11. Intended Use
- Demonstration of analytical logic  
- Controlled scenario exploration  
- Teaching and peer review  
- Foundation for future empirical alignment (outside this release)

---

## 12. Limitations
- Not calibrated to population data  
- Sensitive to regime definitions and design assumptions  
- Interpretability depends on clarity of regime semantics  

---

## 13. Governance & Ethics
- No personal data ingestion in the public documentation release  
- No platform scraping or reverse engineering  
- Clear disclosure boundary between public documentation and private implementation  

---

## 14. Citation
Please cite this release using the machine-readable `CITATION.cff` file and reference the tagged release **v0.1.1-review-ready**.
