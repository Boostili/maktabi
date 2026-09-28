# FUT-501 — Plan compatibility-safe internal identifier migration

- Status: Future
- Milestone: Post-Windows compatibility
- Depends on: stable Windows release

## Outcome

Decide whether and how to migrate internal `@zcode/*`, `.zcode`, `ZCODE_*`, protocol MIME types, RPC names, telemetry keys, theme storage values, plugin IDs, webhook identifiers, and persisted settings.

## Required design

For each identifier, record owner, readers, writers, persistence lifetime, public exposure, dual-read/dual-write period, alias behavior, migration idempotency, rollback, and removal criteria.

## Acceptance

- The plan distinguishes customer-visible defects from harmless implementation names.
- Existing user data and supported integrations have explicit upgrade and rollback scenarios.
- No bulk rename begins before the compatibility matrix is approved.
