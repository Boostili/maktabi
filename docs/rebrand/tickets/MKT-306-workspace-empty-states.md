# MKT-306 — Rebrand the main workspace, model UI, and empty states

- Status: Blocked
- Milestone: Daily-use journey
- Depends on: MKT-102, MKT-201, MKT-305

## Outcome

Remove upstream application identity from the conversation workspace while preserving accurate third-party provider attribution in Advanced Settings.

## Harness scope

- `HARNESS_ROOT/packages/ui/src/v4/ConversationDraftEmptyState.tsx`
- `HARNESS_ROOT/packages/ui/src/assets/Z.svg`
- Model/provider selectors and subscription prompts.
- Shell fallback marks, empty states, banners, ARIA labels, and user-visible error copy.

## Acceptance

- New conversation and workspace fallbacks use approved Maktabi art.
- Default model UI presents Adem/Adem Pro only.
- Z.ai/Start Plan art and purchase prompts are absent from the default experience.
- Explicit third-party provider marks keep their original identity and provenance.
- Empty, loading, error, and narrow-layout states are tested.
