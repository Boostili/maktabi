# MKT-103 — Validate assets, metadata, and checksums

- Status: Blocked
- Milestone: Asset release gate
- Depends on: MKT-101, MKT-102

## Outcome

Prove that the approved asset package is technically safe to integrate and visually correct at every required size.

## Checks

- SVG/XML parsing, view-box consistency, outline-only logo lettering, and absence of external references.
- PNG/ICO dimensions, alpha edges, color count, and native-size legibility.
- Obsidian/White palette compliance and contrast in the near-black UI.
- Production/Preview distinction.
- File naming, checksums, manifest version, and destination completeness.
- Raster and SVG metadata scan for ZCode, Z.ai, authoring-tool paths, and embedded source URLs.

## Acceptance

- A validation report is stored beside the manifest.
- Every manifest entry passes or carries an explicit approved exception.
- MKT-201 and MKT-301 can consume the package without re-exporting or making visual decisions.
