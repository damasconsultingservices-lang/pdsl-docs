# Governance & Disclosure Boundary

## Disclosure Boundary

PDSL public documentation is designed to support reviewability and responsible interpretation while preventing misuse. This repository intentionally excludes:

- engine source code and executable logic
- equations, parameter thresholds, and tuning rules
- operational validation scripts and deployment details

Public materials describe meaning, assumptions, and interpretive discipline — not implementation mechanics.

---

## Semantic Integrity & Hard Gate

PDSL v1.1 model semantics are **frozen**. No update to infrastructure, architecture, or deployment may alter output behavior without a formal semantic version increment.

This commitment is enforced by the `/api/validate` hard gate, which verifies on every deployment that the production engine matches the publicly committed canonical test vector:

- Canonical inputs: `docs/test-vectors/canonical-input-v1.1.json`
- Expected outputs: `docs/test-vectors/canonical-expected-v1.1.json`
- Expected result: `ok: true`

If `/api/validate` returns `ok: false`, the deployment is considered non-conforming and outputs should not be cited.

---

## Versioning

PDSL uses two independent version tracks:

| Track | Current Version | Meaning |
|---|---|---|
| **Model semantics** | v1.1 (frozen) | Stable, citable — all formulas, regimes, fatigue rule, compute() logic |
| **Engine architecture** | v0.2.0 | Internal modularization only — non-semantic |

Public releases are anchored to explicit tags (e.g., `v0.2.0-docs`). Review artifacts should cite the tagged release and reference **v1.1 semantics** for methodological anchoring.

---

## Separation of Tracks

PDSL maintains a deliberate separation between:

| Track | Audience | Contains |
|---|---|---|
| Public docs (`pdsl-docs`) | Academic, policy, review | Conceptual structure, governance, limitations, methods note |
| Private engine (`pdsl`) | Internal / commercial | Source code, deployment, validation scripts |

This separation is a governance choice, not a technical constraint. It protects interpretive integrity by ensuring that public reviewers engage with the conceptual framework on its own terms.

---

## Authorship & Ownership

PDSL is authored and governed by **Frantz Damas**.
