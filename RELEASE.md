# Release Process (Docs)

This repository uses tagged releases to provide stable, citable documentation snapshots anchored to version-specific Zenodo DOIs.

---

## Principles

- Releases are documentation snapshots (review-facing).
- Each release is version-tagged and archived via Zenodo.
- A release must preserve scope boundaries and non-claims.
- Language must remain audit-friendly and avoid overclaiming.
- Citation must reference the tagged release and its corresponding DOI.

---

## Required Checks Before Tagging

Before creating a tagged release:

- `mkdocs build --clean --strict` passes without errors
- Navigation renders correctly on GitHub Pages
- `CITATION.cff` is updated and reflects the release version
- Zenodo DOI is reserved or generated and matches the release
- Changelog is updated
- “How to Cite” page references the correct version tag and DOI

---

## Tag Format

Use semantic versioning with a review anchor suffix when relevant:

Example:
v0.1.2-review-ready

Tags must match:

- The version listed in `CITATION.cff`
- The Zenodo DOI archive metadata
- The GitHub Release title
- The changelog entry

---

## Release Contents

Each documentation release should include:

- Model Card (scope and non-claims)
- Methods Note (interpretive logic)
- Review Protocol (discipline and review boundaries)
- Governance and Limitations (guardrails)
- Policy documentation
- Citation guidance

A release must reflect a coherent documentation state suitable for citation and review.

---

## DOI and Repository Reference

Each tagged release must include:

**DOI (Zenodo, citable archive):**  
The DOI corresponding to the specific tagged version (e.g., v0.1.2-review-ready).

**Repository:**  
https://github.com/damasconsultingservices-lang/pdsl-docs

The Zenodo DOI serves as the authoritative citation anchor for the tagged documentation snapshot.  
Each release version must reference its matching DOI.

---

## Post-Release Verification

After publishing:

- Confirm the GitHub Release description includes the correct DOI
- Confirm GitHub Pages deploys successfully
- Confirm citation instructions reference the release tag and DOI
- Confirm Zenodo metadata matches the tagged version
- Confirm README badge links to the correct DOI
- Confirm changelog reflects the release accurately

---

This document defines the release discipline for documentation snapshots only.  
It does not govern simulation engine behavior or model architecture.
