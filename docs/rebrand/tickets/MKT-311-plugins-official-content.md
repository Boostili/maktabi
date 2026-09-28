# MKT-311 — Replace or disable marketplace and official-content routes

- Status: Blocked
- Milestone: Extensibility
- Blocker: Maktabi marketplace/CDN decision and content ownership

## Outcome

Prevent Maktabi from presenting ZCode official plugins, promotional art, or CDN content as its own.

## Harness scope

- `HARNESS_ROOT/packages/shared/src/plugin-marketplaces.ts`
- `HARNESS_ROOT/packages/ui/src/v4/featureSuggestedPrompts.ts`
- `HARNESS_ROOT/apps/zcode-cli/packages/bootstrap/src/app/official-plugin-definitions.ts`
- Official-content URLs, marketplace IDs, banners, thumbnails, and install flows.

## Rules

- Either provide a Maktabi-owned marketplace/CDN contract or disable official-store surfaces.
- User-added third-party sources remain distinct and accurately labeled.
- Do not copy upstream promotional artwork without an explicit license and product decision.

## Acceptance

- Network inspection shows no request to `cdn-zcode.z.ai` or upstream marketplace endpoints.
- Empty/disabled store states are coherent in English, French, and Arabic.
- Installed third-party plugin provenance remains visible.
