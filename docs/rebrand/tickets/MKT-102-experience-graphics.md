# MKT-102 — Produce experience graphics

- Status: In progress
- Milestone: Experience assets
- Depends on: MKT-002

## Outcome

Create the owned graphics needed for launch, first run, account/model connection, completion, and an empty conversation in the approved black-and-white system.

## Deliverables

- Startup/loading badge and reduced-motion treatment.
- Welcome/login hero.
- Adem and Adem Pro connection illustration.
- Ready/completion graphic.
- New-conversation empty-state art.
- Reusable website/login banner.

## Future harness routes

- `HARNESS_ROOT/packages/ui/src/assets/`
- `HARNESS_ROOT/packages/ui/src/onboarding/assets/`
- Shared components that replace `ZCodeAboutLogo.tsx`, startup drawing, and inline empty-state SVG.

## Rules

- Use Obsidian and White only; functional UI neutrals may appear outside the artwork.
- Do not bake English, French, or Arabic text into illustrations.
- Provide accessible descriptions and reduced-motion behavior specifications.
- Do not use Z.ai/ZCode CDN artwork or the user-supplied raster as production artwork.

## Acceptance

- Each graphic has desktop dark-theme composition, small-window behavior, and a documented runtime route.
- Artwork contains no external URLs, unlicensed elements, or upstream marks.
- Review boards show the assets in the actual near-black application context.

## Progress

Generated first-pass owned SVG exports for startup, welcome, model connection, ready, empty conversation, and the reusable banner under `branding/maktabi/exports/app/`. The companion `EXPERIENCE_GRAPHICS_GUIDE.md` records runtime routes, accessible descriptions, small-window behavior, and reduced-motion behavior. These exports are ready for visual review before runtime copies are introduced in the harness.
