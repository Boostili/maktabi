# MKT-309 — Replace or disable sharing, web remote, and public deep links

- Status: Blocked
- Milestone: Cross-device journey
- Blocker: Maktabi share, web-remote, and protocol migration contracts

## Outcome

Move public `zcode://` and ZCode-hosted share/remote experiences to Maktabi-owned contracts without breaking local session boundaries.

## Harness scope

- `HARNESS_ROOT/packages/web/src/share/ConversationShareLandingPage.tsx`
- `HARNESS_ROOT/packages/web/src/main.tsx`
- `HARNESS_ROOT/packages/desktop/src/main/desktopOAuthDeepLink.ts`
- `HARNESS_ROOT/packages/ui/src/WebRemoteControlDialog.tsx`
- `HARNESS_ROOT/packages/ui/src/WorkspaceWebRemoteControlTrigger.tsx`
- Shared protocol and endpoint configuration.

## Rules

- Public protocol is `maktabi://`; any legacy alias requires an explicit transition and security policy.
- Preserve the architectural difference between desktop-continuous and web-remote-replayable links.
- Disable share/import and remote entry points until the Maktabi service exists.

## Acceptance

- Auth, share import, malformed link, wrong-host, expired link, and protocol-registration scenarios are tested.
- Web pages, titles, download buttons, and callbacks use Maktabi identity.
- No Maktabi build sends share or remote-control data to upstream services.
