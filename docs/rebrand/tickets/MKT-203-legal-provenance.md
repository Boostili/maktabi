# MKT-203 — Add legal presentation and provenance

- Status: Ready after legal review
- Milestone: Legal

## Outcome

Present Maktabi ownership while preserving all required upstream and third-party notices, including the approved “Based on ZCode” entry.

## Harness scope

- `HARNESS_ROOT/LICENSE`
- `HARNESS_ROOT/NOTICE.md`
- `HARNESS_ROOT/THIRD-PARTY-NOTICES.md`
- `HARNESS_ROOT/packages/desktop/src/main/about.ts`
- Distributed notice files and About/legal links.

## Rules

- Preserve the Apache-2.0 license and legally required attribution.
- Put “Based on ZCode” in legal/provenance surfaces, not ordinary navigation.
- Preserve third-party icon, font, binary, and provider-logo notices.
- Regenerate notices when dependencies or redistributed assets change.

## Acceptance

- Source and installed artifacts contain the required notices.
- About identifies Maktabi Agent and exposes legal/provenance access.
- No legal text falsely implies Z.ai or ZCode operates Maktabi.
- Release owner records legal review; this ticket is not itself legal advice.
