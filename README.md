# Public Diplomacy Simulation Lab (PDSL) — Public Docs
**Release:** v0.1.1-review-ready  
**Repository type:** Public, review-facing documentation (no engine)

## Executive Summary
The **Public Diplomacy Simulation Lab (PDSL)** is a **deterministic, theory-constrained simulation framework** built to support **controlled scenario reasoning** in public diplomacy and digitally mediated influence contexts. This public repository contains **review-facing documentation** that enables academic, institutional, and policy stakeholders to understand PDSL’s **scope, assumptions, interpretive logic, and governance discipline**—without exposing the simulation engine, source code, or proprietary mechanics.

PDSL **does not** produce empirical causal estimates, predictions, or forecasts. Instead, it translates structured analytical inputs (e.g., exposure, threat framing with saturation, identity salience, AI literacy, time) into three governed outcome channels interpreted through a regime-based analytical framework:

- **APR — Algorithmic Persuasion Risk**
- **IAS — Identity Alignment Shift**
- **PST — Policy Support via Threat Framing**

Outputs are **interpretive constructs** for comparative reasoning, not measurements of real-world effects.

## What This Repo Contains
- **Model Card** (scope, intended use, assumptions, limitations, ethics)
- **Review Protocol** (how to evaluate the documentation and interpret outputs)
- **Policy-Facing Methods Overview** (high-level design logic for non-technical readers)
- **Figure & Output Interpretation Notes** (how to read results responsibly)
- **Governance & Citation Materials** (versioning, authorship, acceptable use)

📄 Documentation index: `docs/index.md`

## What This Repo Does *Not* Contain
To preserve research integrity and prevent misuse, this repository does **not** include:
- Simulation engine or source code
- Parameter logic, equations, regime thresholds, or tuning details
- Internal validation scripts, diagnostics, or deployment instructions
- API endpoints, operational gates, or infrastructure configuration

Those components are maintained separately in a restricted repository.

## How to Review (Conceptual)
Reviewers should:
1. Start with `docs/model-card.md` for scope, assumptions, and limits.
2. Use `docs/review-protocol.md` to follow the review discipline.
3. Interpret APR/IAS/PST through `docs/figures/regime-interpretation.md`.
4. Cite the release using `CITATION.cff` (avoid citing untagged commits).

## Licensing
- Academic/review use: see `LICENSE`
- Commercial use: requires a separate agreement — see `COMMERCIAL_LICENSE.md`

## Ownership & Attribution
PDSL is authored and governed by **Frantz Damas**. All public documentation releases are versioned and review-anchored.

---
**Release anchor:** `v0.1.1-review-ready`
