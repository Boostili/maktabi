# MKT-101 — Produce the Windows icon and shared export matrix

- Status: Complete
- Milestone: Windows assets
- Depends on: MKT-002

## Outcome

Generate the complete Windows-ready asset family from the approved masters while keeping those exports in the Maktabi repository until implementation begins.

## Deliverables

- PNG ladder at 16, 24, 32, 48, 64, 128, 256, 512, and 1024 px.
- Multi-resolution production and Preview ICO files.
- Window/taskbar, tray, installer/uninstaller, installer-header, favicon, README/avatar, and web exports.
- Preview treatment that remains legible at 16 px and visually distinct beside production.

## Future harness routes

- `HARNESS_ROOT/packages/desktop/build/icon.ico`
- `HARNESS_ROOT/packages/desktop/build/icon_windows.png`
- `HARNESS_ROOT/packages/desktop/build/icon_installer.ico`
- `HARNESS_ROOT/packages/desktop/build/icon_installer.png`
- `HARNESS_ROOT/packages/desktop/build/icons/*.png`
- `HARNESS_ROOT/packages/web/public/favicon.ico`
- `HARNESS_ROOT/public/logo/icons/*`

## Acceptance

- Every export has dimensions, checksum, color mode, version, approval state, and exact route-map destination.
- Icons remain recognizable at native size on light and dark Windows chrome.
- ICO contents match the documented ladder and contain no upstream pixels or metadata.
- No runtime file is changed by this ticket.

## Completion evidence

Completed 2026-09-27. The approved production and Preview masters were rasterized into the 16–1024 px PNG ladder, multi-resolution Windows ICO files, Windows aliases, favicon, and 1024 px web/README export under `branding/maktabi/exports/`. `branding/maktabi/inventory/ASSET_MANIFEST.json` records dimensions, color mode, SHA-256 checksums, version, approval state, source, and exact route-map destination for every export. The validator checked RGBA dimensions, recomputed all checksums, verified the production/Preview ICO ladders and embedded PNG dimensions, and found no upstream/source metadata; visual checks at 16px and 256px on light and near-black fields confirmed legibility and Preview distinction. The harness remains unchanged; runtime copying is deferred to the consuming implementation tickets.
