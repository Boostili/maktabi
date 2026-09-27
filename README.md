# Maktabi Product Workspace

This repository owns the Maktabi brand sources, product decisions, specifications, inventories, and implementation tickets. It deliberately does not contain a second copy of the application source.

## Workspace layout

The two sibling repositories have different jobs:

```text
D:\Zai01\
|-- zcode-harness\   # the one working application repository
`-- maktabi\         # this brand, specification, and ticket repository
```

`HARNESS_ROOT` means `../zcode-harness`. Any application path in Maktabi documentation is resolved from that root. For example:

```text
HARNESS_ROOT/packages/desktop/build/icon.ico
= D:\Zai01\zcode-harness\packages\desktop\build\icon.ico
```

## Working rule

- Edit application code only in `zcode-harness/`.
- Keep editable brand masters and planning records only in `maktabi/`.
- Export approved copies into the harness only through an implementation ticket.
- Do not create another application checkout inside `maktabi/`.
- The Maktabi repository remains local until ticket `MKT-001` connects the approved GitHub destination.

## Start here

- Product vocabulary and boundaries: `CONTEXT.md`
- Rebrand architecture: `docs/rebrand/REBRAND_ARCHITECTURE.md`
- Full plan: `docs/rebrand/REBRAND_PLAN.md`
- Asset, text, and link routes: `branding/maktabi/inventory/ASSET_ROUTE_MAP.md`
- Windows ticket graph: `docs/rebrand/TICKETS.md`
- Current identity-system work: `docs/rebrand/phase-2/TICKETS.md`

No runtime assets or application code have been replaced yet.

