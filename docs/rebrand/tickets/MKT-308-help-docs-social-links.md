# MKT-308 — Route help, docs, support, feedback, and social links

- Status: Blocked
- Milestone: Help journey
- Blocker: approved live URL and email catalogue

## Outcome

Ensure every help or community action opens an owned, live Maktabi destination—or is disabled until one exists.

## Harness scope

- `HARNESS_ROOT/packages/ui/src/lib/productDocs.ts`
- `HARNESS_ROOT/config/default.json`
- Desktop application menus and About links.
- README badges, support/community calls to action, privacy, terms, status, and feedback.

## Required inputs

Documentation, downloads, support email, feedback, privacy, terms, service status, community/social destinations, and ownership for each.

## Acceptance

- An automated link inventory covers every clickable app-owned destination.
- Every enabled route returns the expected Maktabi page and preserves locale where applicable.
- No action opens ZCode, Z.ai, Zhipu Feishu, upstream Discord, or a placeholder page.
- Unavailable destinations are hidden or clearly disabled, not silently redirected.
