# MKT-305 — Define and implement Adem and Adem Pro

- Status: Blocked
- Milestone: Model journey
- Depends on: MKT-304
- Blocker: model IDs, API/streaming schema, context limits, quotas, and entitlement rules

## Outcome

Make Adem and Adem Pro the only first-party model choices, backed by Maktabi services and internally routed through OmniRoute.

## Harness scope

- `HARNESS_ROOT/config/provider/zcode-builtin.json`
- `HARNESS_ROOT/packages/shared/src/model-provider-family.ts`
- Provider/model services and selectors.
- `HARNESS_ROOT/apps/zcode-cli/packages/adapters/src/model/official-coding-plan-gateway.ts`
- Maktabi model artwork from MKT-002/MKT-102.

## Product rules

- Adem: Low and Moderate thinking.
- Adem Pro: Low, Moderate, High, and Max thinking.
- OmniRoute is an implementation name, not a user-facing provider.
- Compatible third-party configuration moves under Advanced Settings.

## Acceptance

- Entitled users see only valid model/thinking combinations.
- Unsupported or expired entitlement states fail clearly and do not fall back to Z.ai.
- Streaming, cancellation, retry, quota, and error mapping are specified and tested.
- Desktop and CLI resolve the same catalogue truth.
