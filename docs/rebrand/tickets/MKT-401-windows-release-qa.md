# MKT-401 — Verify the complete Windows customer journey

- Status: Blocked
- Milestone: Windows release gate
- Depends on: MKT-203 and implemented Windows tickets MKT-301 through MKT-313

## Outcome

Prove a fresh Windows user can install, launch, onboard, authenticate, use Adem, get help, update, and uninstall without encountering accidental upstream identity or dead links.

## Scenarios

- Clean production install and first launch.
- Preview side-by-side with production.
- Upgrade over a prior Maktabi build and documented behavior over an existing ZCode profile.
- English, French, Arabic/RTL, dark, light, Windows scaling, reduced motion, and narrow window.
- Login success/denial/expiry/offline, entitlement refresh, Adem/Adem Pro selection, and thinking levels.
- Taskbar, tray, shortcuts, Start menu, protocol, About, file properties, diagnostics, and uninstall.
- Help, legal, payment, share, update, plugin, and supported bot routes.

## Required verification

- Harness package tests and E2E scenarios selected from current package scripts.
- `pnpm typecheck`
- `pnpm lint`
- `pnpm fmt:check`
- `pnpm architecture:check --changed`
- Installer build plus inspection of installed/unpacked artifacts.

## Acceptance

- Results are recorded with build version, Windows version, language/theme, evidence, and any approved exceptions.
- Production and Preview coexist without identity, protocol, update, or data collisions.
- No unresolved blocker is hidden behind a fallback upstream service.
