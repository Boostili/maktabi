# MKT-003 — Maintain the asset, text, link, and compatibility inventory

- Status: In progress
- Milestone: Governance
- Baseline: `HARNESS_ROOT` v3.14.3 (`29628c9`)

## Outcome

Keep one auditable map for every customer-facing graphic, brand string, clickable destination, public identifier, and intentionally preserved compatibility name.

## Scope

- Maintain `branding/maktabi/inventory/ASSET_ROUTE_MAP.md`.
- Rescan `HARNESS_ROOT` whenever its baseline changes.
- Classify each result as replace, remove, disable, keep/review, blocked, legal, internal, or false positive.
- Include code-drawn SVG/CSS/Canvas art, remote images, ARIA labels, HTML titles, installer metadata, public logs, user agents, and network destinations.
- Track the v3.14.3 bots/remote-control UI and channel icons.

## Acceptance

- The route map records the exact harness baseline and `HARNESS_ROOT` convention.
- Every shipped upstream-brand match is either routed to a ticket or explicitly preserved with a reason.
- New binary/channel assets have a provenance disposition.
- The final audit can mechanically compare its findings with this inventory.
