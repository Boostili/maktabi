# MKT-304 — Define and implement the Maktabi account contract

- Status: Blocked
- Milestone: Account journey
- Blocker: authorization, callback, token/session, user-info, logout, refresh, and error contracts

## Outcome

Replace Z.ai/BigModel login with a Maktabi-owned authorization flow through `maktabi.space` and `maktabi://auth/callback`.

## Harness scope

- `HARNESS_ROOT/packages/shared/src/zcodeEndpoint.ts`
- `HARNESS_ROOT/packages/services/src/oauth/providers/`
- `HARNESS_ROOT/packages/ui/src/WelcomeScreen.tsx`
- `HARNESS_ROOT/packages/web/src/auth/`
- `HARNESS_ROOT/packages/desktop/src/main/desktopOAuthDeepLink.ts`
- CLI authentication adapters and login command.

## Required specification

Define state/PKCE handling, callback ownership, token storage, refresh, logout, account identity, entitlements, expiration, offline behavior, redaction, and rollback. Preserve the existing desktop/web host boundaries.

## Acceptance

- Login, callback validation, restart persistence, refresh, logout, denial, expiry, and offline scenarios are tested.
- Secrets never enter logs, examples, or renderer-owned storage.
- No default auth button or failure path opens an upstream account service.
- Endpoint configuration fails closed when Maktabi services are unavailable.
