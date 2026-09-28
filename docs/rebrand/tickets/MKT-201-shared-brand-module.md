# MKT-201 — Add the shared Maktabi brand module and tokens

- Status: Blocked
- Milestone: UI foundation
- Depends on: MKT-002, MKT-101

## Outcome

Give desktop and web UI one public source for Maktabi marks, product names, brand colors, accessible labels, and approved asset imports.

## Harness scope

- `HARNESS_ROOT/packages/ui/src/` public asset/component entry points.
- Shared product-name/configuration surfaces used by desktop and web.
- Focused tests for variants, accessible names, and missing-asset failures.

## Rules

- One shared component owns the Latin runtime symbol/lockup and Preview variants. Arabic and bilingual lockups remain collateral-only and are not imported by the final desktop app.
- UI code does not import arbitrary files from the Maktabi repository.
- Stored compatibility IDs such as `zai-dark` may remain internal while displayed labels change.
- Platform differences flow through existing public services, not direct `window.zcode` access.

## Acceptance

- Desktop and web can render approved variants through a documented API.
- No new duplicate logo drawing or product-name constant is introduced.
- Existing third-party provider marks remain isolated from app identity.
- Architecture, typecheck, lint, and relevant component tests pass.
