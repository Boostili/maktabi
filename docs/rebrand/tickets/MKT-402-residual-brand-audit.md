# MKT-402 — Audit residual brand, visuals, artifacts, and routes

- Status: Blocked
- Milestone: Final release gate
- Depends on: MKT-401

## Outcome

Close the rebrand with a reproducible scan of source and distributed artifacts, including the kinds of leftovers a text-only search misses.

## Scan set

- `ZCode`, `zcode`, `Z.AI`, `Z.ai`, `z.ai`, `zai-org`, `zcode.z.ai`, `chat.z.ai`, `api.z.ai`, `cdn-zcode.z.ai`, `dev.zcode.app`, and `zcode://`.
- SVG metadata, raster OCR/manual review, ICO resources, executable/file properties, installer strings, shortcuts, ARIA labels, document titles, user agents, logs offered to users, and network requests.
- Every clickable button/link in the installed app and first-run flow.

## Dispositions

Every match is classified as replace, remove, disable, legal, internal compatibility, third-party provider, test fixture, false positive, or release defect. Unclassified results fail the gate.

## Acceptance

- The audit report points each allowed result to the route map or compatibility plan.
- No customer-facing accidental upstream identity remains.
- Required “Based on ZCode” and license notices are present.
- All enabled links resolve to approved destinations and no public request silently reaches an upstream product service.
