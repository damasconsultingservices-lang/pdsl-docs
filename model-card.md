# PDSL Model Card (Public)

## 1. Model Name
**Public Diplomacy Simulation Lab (PDSL)** — public documentation release.

## 2. Version / Release Anchor
**v0.1.1-review-ready**

## 3. Purpose
PDSL is a deterministic, theory-constrained simulation framework designed to support **controlled scenario reasoning** in public diplomacy contexts. It is intended to help analysts and reviewers compare policy levers and narrative conditions under explicitly stated assumptions.

## 4. Intended Users
- Academic reviewers and researchers
- Policy analysts and strategic communication teams
- Educators using simulation-based learning

## 5. Non-Intended Uses (Explicit Non-Claims)
PDSL is not designed for:
- empirical causal inference
- forecasting or prediction of real-world behavior
- platform reverse engineering or surveillance
- individualized targeting, profiling, or manipulation

## 6. Conceptual Inputs (High-Level)
PDSL is parameterized using abstract inputs that represent:
- exposure intensity
- threat framing intensity (with saturation)
- identity salience
- AI literacy / media literacy
- time or iteration horizon

This public release describes inputs conceptually and does not disclose thresholds, equations, or engine-specific mechanics.

## 7. Outputs (Governed Outcome Channels)
PDSL produces three outcome channels intended for interpretive, comparative analysis:
- **APR — Algorithmic Persuasion Risk**
- **IAS — Identity Alignment Shift**
- **PST — Policy Support via Threat Framing**

Outputs are interpreted through a **regime-based analytical framework**.

## 8. Interpretability
Outputs are not standalone scores. Interpretation requires:
- understanding scope and limitations
- reading outputs through the regime logic explained in the interpretation guide
- respecting non-claims and disclosure boundaries

## 9. Assumptions
- deterministic behavior under identical inputs
- theory-constrained regime interpretation
- analytical abstraction from real platform mechanics

## 10. Limitations
- does not estimate causal effects
- does not incorporate platform-specific proprietary signals
- sensitivity depends on assumed input ranges
- outputs are comparative constructs, not empirical measurements

## 11. Governance & Ethics
- no ingestion of personal data in the public documentation release
- no scraping or reverse engineering
- disclosure boundary: public materials explain meaning and discipline, not mechanics

## 12. Citation
Use `CITATION.cff` to cite this release and avoid citing untagged commits.
