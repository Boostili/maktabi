# Maktabi Brand Source

Status: Phase 3 export matrix approved; source masters remain canonical
Version: 0.4  
Last reviewed: 2026-09-24

This directory is the source of truth for Maktabi visual identity. Files under application packages are deployment copies. Every approved export must be traceable back to an editable master here through `inventory/ASSET_ROUTE_MAP.md`.

## Brand idea

Maktabi means “my office” or “my workspace.” The lead identity treats that idea as an organized personal library: a rounded workspace containing one leaning volume and two upright volumes. The same rhythm can be read as books, files, or an open-book gesture. It is designed to extend from coding into education, law, finance, and other professional work without presenting a profession-specific symbol.

The character is:

- Precise and dependable.
- Warm enough for daily personal work.
- Algerian through proportion, light, and geometry rather than flags, maps, monuments, or costume.
- Professional without appearing governmental or ceremonial.
- Technological without sparkles, circuit clichés, or a generic chatbot face.

## Approved identity constants

| Item | Value |
| --- | --- |
| Brand | Maktabi |
| Product | Maktabi Agent |
| Arabic name | مكتبي |
| Obsidian | `#09090B` |
| White | `#FFFFFF` |
| Latin type | Manrope |
| Arabic type | Tajawal Bold |
| Default environment | Near-black |
| Mark construction | Rounded-square workspace with a three-volume book/file rhythm |

Gray is a functional interface neutral and does not create an additional brand accent. Purple and orange/gold from earlier references and explorations are not part of the confirmed Maktabi palette.

The primary icon treatment is confirmed: an Obsidian rounded square containing White books. The colors are not inverted for the standard application icon.

## Directory contract

```text
branding/maktabi/
├── README.md
├── source/
│   ├── concepts/          # Review-stage vector directions
│   └── *.svg              # Canonical production masters
├── exports/
│   ├── app/               # Shared application symbols and lockups
│   ├── windows/           # ICO and Windows PNG outputs
│   ├── macos/             # Future desktop exports
│   ├── web/               # Favicons and web lockups
│   ├── social/            # Avatar and banner exports
│   └── future-ios/        # Reusable masters; no current iOS app
├── references/            # Approved visual references and licenses
└── inventory/
    ├── ASSET_MANIFEST.json # Version and approval registry
    └── ASSET_ROUTE_MAP.md  # Source, export, consumer, and status
```

Phase 2 rules and acceptance gates live in `docs/rebrand/phase-2/PHASE_2_BRAND_ASSET_SYSTEM_SPEC.md`.

## Concept directions

### 01 — Threshold M

File: `source/concepts/maktabi-agent-concept-01-threshold.svg`

A direct M constructed as two mirrored structural bays around a gold doorway. Rejected on 2026-09-24; retained only as design history.

### 02 — Courtyard M

File: `source/concepts/maktabi-agent-concept-02-courtyard.svg`

A wider, calmer mark with a central work surface and open courtyard. Rejected on 2026-09-24; retained only as design history.

### 03 — Folded Workspace

File: `source/concepts/maktabi-agent-concept-03-folded-workspace.svg`

Mirrored planes fold inward to form an M and a central route. Rejected on 2026-09-24; retained only as design history.

### 04 — Book / Workspace

File: `source/concepts/maktabi-agent-concept-04-book-workspace.svg`

The confirmed direction uses the supplied open-book/folder image only as a compositional reference. The artwork is recreated on a 120-unit grid with a 29-unit corner radius, three identical 18 × 68-unit modules, 29-unit center spacing, and one controlled 10-degree lean. The approved treatment is an Obsidian container with White books.

Concepts 01–03 are rejected and cannot be promoted. Concept 04 is confirmed. Its board still uses live font references for review; the final wordmark will be converted to vector outlines before production export.

## Logo rules

- Preserve the rounded container, the leaning-left volume, and the two-upright-volume rhythm.
- Construct every volume from the same 18 × 68-unit module; do not redraw or stretch individual books.
- Keep centers on a 29-unit horizontal rhythm. Only the first module may rotate, at 10 degrees.
- Use flat fills only. Do not add gradients, shadows, bevels, glow, or texture to the core logo.
- Use the symbol alone below 120 px lockup width.
- Test the symbol at 64, 32, 24, and 16 px before approval.
- Keep clear space of at least one internal module around every side of the mark.
- Use an Obsidian container with White books for the primary mark.
- On a dark application background, preserve the Obsidian container and use a subtle neutral boundary only when needed for silhouette separation.
- On a light background, use the unchanged Obsidian/White primary mark.
- One-color black and white variants are required for system contexts.
- Do not add Algerian flags, crescents, maps, landmarks, code brackets, bot faces, or AI sparkles to the symbol.

## Typography rules

- Manrope is the reference for Latin marketing, banners, and product lockups.
- Tajawal Bold is the reference for Arabic graphic collateral and construction of `مكتبي`.
- The application keeps its compact system UI and mono stacks during the first rebrand implementation.
- Final logo lettering is delivered as outlines plus a separately editable text reference.
- Arabic layouts use proper RTL composition: the `مكتبي` wordmark sits on the left and the symbol sits on the right; do not mirror the Latin wordmark mechanically.
- Arabic and bilingual lockups are graphic collateral only. The final desktop app uses Latin graphic assets; Arabic localization does not import Arabic logo artwork.

## Usage rules

- Keep at least `1x` clear space on every side of a symbol or complete lockup, where `1x` is one 18-unit book module.
- Use the symbol alone below the `120 px` Latin lockup minimum; the Arabic collateral lockup follows its approved proof minimum.
- Preserve the approved aspect ratio, module geometry, and 10-degree lean. Do not stretch, redraw, mirror, or rearrange the books.
- Use the primary Obsidian container with White books on light and near-black fields. Pure-black separation belongs to the containing layout, not a baked-in logo stroke.
- Use one-color dark or light variants only where the consuming system requires them; their book shapes are transparent cutouts.
- Preview uses the approved external four-corner bracket. Do not replace it with an error badge, notification dot, gradient, or text-only label.
- Adem and Adem Pro are subordinate model marks. Thinking levels remain text, and OmniRoute has no customer-facing mark.
- Arabic and bilingual lockups are collateral-only. The final desktop app imports Latin graphic assets only.

Incorrect usage includes arbitrary rotation or distortion, recoloring, gradients, shadows, mirroring, uneven book widths, extra badges, flags, slashes, and replacing the approved symbol with a provider mark.

## Illustration language

Experience graphics use the same book/file rhythm as the mark:

- Obsidian fields with White geometry applied to shelves, files, pages, and workspace panels.
- Limited neutral white/gray for content and accessibility.
- Quiet depth made with scale, overlap, and negative space rather than gradients.
- Accurate interface diagrams for instructional steps.
- Subtle Algerian spatial cues through shelving, screens, pattern, and proportion rather than literal national symbols.
- People may represent diverse Algerian professionals in marketing artwork; first-run product claims stay aligned with shipped capabilities.

## Model identity

Adem uses a small geometric A derived from the selected Maktabi grid. Adem Pro uses the same mark with a restrained white frame or four-point structural modifier. Thinking levels remain text labels:

| Model | Levels |
| --- | --- |
| Adem | Low, Moderate |
| Adem Pro | Low, Moderate, High, Max |

OmniRoute is the internal routing layer and receives no customer-facing provider logo in first run.

## Naming convention

Master and export filenames use lowercase kebab-case:

```text
maktabi-agent-mark-primary.svg
maktabi-agent-lockup-latin-horizontal.svg
maktabi-agent-lockup-ar-horizontal.svg
maktabi-agent-lockup-bilingual.svg
maktabi-agent-icon-production-256.png
maktabi-agent-icon-preview-256.png
maktabi-agent-onboarding-models-dark.svg
adem-model-mark.svg
adem-pro-model-mark.svg
```

Avoid dates in stable runtime filenames. Version and approval information belongs in the future asset manifest; concept filenames retain their numbered direction.

## Approval gates

1. Confirm Concept 04 geometry and primary colors. **Complete: 2026-09-24.**
2. Approve the production symbol, wordmark geometry, and small-size exports.
3. Approve Latin, Arabic, and bilingual lockups.
4. Approve production and Preview icons.
5. Approve Adem family marks.
6. Approve onboarding and banner illustration system.
7. Approve the full export manifest before runtime replacement.

An asset is production-ready only when its source, export, target, dimensions, variant, license/provenance, and approval status are present in the route map or manifest.
