# MKT-310 — Replace update, download, and release infrastructure

- Status: Blocked
- Milestone: Release delivery
- Blocker: artifact host, signed manifest contract, channels, publisher/signing identity, and rollback policy

## Outcome

Deliver production and Preview builds from Maktabi-owned release infrastructure and prevent upstream update/download endpoints from being used.

## Harness scope

- `HARNESS_ROOT/packages/desktop/src/main/remoteCdn.ts`
- `HARNESS_ROOT/packages/desktop/electron-builder.config.js`
- Release scripts, manifests, environment configuration, web download calls to action, and force-update UI.

## Acceptance

- Production and Preview query separate approved channels.
- Manifests and artifacts are signed/verified according to the release specification.
- Disabled-update development builds say so clearly and never fall back upstream.
- Upgrade, rollback/failure, offline, corrupt artifact, and channel-switch scenarios are tested.
- Download pages and filenames use Maktabi Agent identity.
