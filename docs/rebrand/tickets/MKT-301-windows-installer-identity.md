# MKT-301 — Rebrand the Windows installer and operating-system identity

- Status: Blocked
- Milestone: Windows packaging
- Depends on: MKT-101; publisher/signing decision

## Outcome

Make install, upgrade, side-by-side Preview, shortcuts, file properties, protocol registration, and uninstall consistently identify Maktabi Agent.

## Harness scope

- `HARNESS_ROOT/packages/desktop/scripts/desktop-product-identity.mjs`
- `HARNESS_ROOT/packages/desktop/electron-builder.config.js`
- `HARNESS_ROOT/packages/desktop/package.json`
- `HARNESS_ROOT/packages/desktop/build/installer.nsh`
- `HARNESS_ROOT/packages/desktop/build/` approved icon routes.

## Product values

- Production: `Maktabi Agent`, app ID `space.maktabi.agent`, machine name `maktabi-agent`.
- Preview: `Maktabi Agent Preview`, distinct app ID/name/icon and install location.
- Public protocol: `maktabi://`, subject to MKT-309 migration rules.

## Acceptance

- Clean install, upgrade, Preview coexistence, Start menu, shortcuts, taskbar grouping, file metadata, protocol entry, and uninstall show approved Maktabi identity.
- Installer logs and visible error text contain no upstream product name.
- Signing/publisher metadata is truthful; unsigned development builds are clearly distinguished.
- Packaging tests and an installed-artifact inspection pass on Windows.
