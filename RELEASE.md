# Release Process (Docs)

This repository uses tagged releases to provide stable, citeable documentation snapshots.

## Principles
- Releases are documentation snapshots (review-facing).
- A release must preserve “scope and non-claims.”
- Language must remain audit-friendly and avoid overclaiming.

## Required checks before tagging
1) `mkdocs build --clean --strict` passes
2) Navigation renders correctly on GitHub Pages
3) CITATION is correct and references the release tag
4) Changelog updated

## Tag format
- Use semantic tags with a review anchor suffix when relevant:
  - `v0.1.1-review-ready`

## Release contents
A release should reflect:
- Model Card (scope/non-claims)
- Methods Note (interpretive logic)
- Review Protocol (discipline)
- Governance + Limitations (guardrails)
- Policy + Cite sections

## Post-release verification
- Confirm site loads from GitHub Pages
- Confirm citation instructions reference the tag
