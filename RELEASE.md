# Release Process (Docs)

This repository uses tagged releases to provide stable, citable documentation snapshots anchored to a Zenodo DOI.

---

## Principles

- Releases are documentation snapshots (review-facing).
- Each release is version-tagged and archived via Zenodo.
- A release must preserve scope boundaries and non-claims.
- Language must remain audit-friendly and avoid overclaiming.
- Citation must reference the tagged release and corresponding DOI.

---

## Required checks before tagging

Before creating a tagged release:

- `mkdocs build --clean --strict` passes
- Navigation renders correctly on GitHub Pages
- `CITATION.cff` is updated and reflects the release version
- Zenodo DOI is reserved (if applicable) and matches the release
- Changelog is updated
- “How to Cite” page references the correct DOI

---

## Tag format

Use semantic tags with a review anchor suffix when relevant:

v0.1.2-review-ready

Tags must match:

- The version listed in `CITATION.cff`
- The Zenodo DOI archive
- The GitHub Release title

---

## Release contents

A release should reflect:

- Model Card (scope / non-claims)
- Methods Note (interpretive logic)
- Review Protocol (discipline)
- Governance + Limitations (guardrails)
- Policy + Cite sections

---

## DOI and Repository Reference

Each release must include:

**DOI (Zenodo, citable archive):**  
https://doi.org/10.5281/zenodo.18732275  

**Repository:**  
https://github.com/damasconsultingservices-lang/pdsl-docs  

The Zenodo DOI serves as the authoritative citation anchor for the tagged documentation release.

---

## Post-release verification

After publishing:

- Confirm GitHub Release description includes the DOI
- Confirm GitHub Pages site loads correctly
- Confirm citation instructions reference the release tag and DOI
- Confirm Zenodo record metadata matches the tagged version
- Confirm README badge links to the correct DOI
