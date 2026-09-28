# Maktabi Rebrand Plan

Status: Phase 2 complete; Phase 3 ready
Implementation state: Phase 2 source masters, proofs, and frozen manifest complete; runtime replacement not started
Last reviewed: 2026-09-27

## Goal

Deliver a Windows-first Maktabi Agent release with a complete visual identity, Maktabi-owned customer destinations, and no accidental ZCode/Z.ai branding in the customer journey. Preserve compatibility-sensitive internals until their own migration is specified.

## Current gate and delivery route

Discovery/grilling, the repository inventory, and logo selection are complete. Because the complete rebrand is a multi-session build, the next workflow is:

1. Convert this plan and `REBRAND_ARCHITECTURE.md` into implementation-ready specifications with product rules, owners, interfaces, and acceptance scenarios.
2. Split those specifications into blocker-first tracer-bullet tickets, with explicit dependency edges.
3. Implement one ticket at a time, adding tests before behavior changes and reviewing each diff against both repository standards and its specification.

The immediate specification is the Phase 2 brand asset system. It covers the production symbol, Latin/Arabic/bilingual wordmarks, clear-space and minimum-size rules, Preview modifier, Adem marks, and the export manifest. Runtime asset replacement remains out of scope until that specification and its outputs are approved.

## Work sequence

### Phase 0 — Discovery and decisions

Completed in this task:

- Product hierarchy, visual character, palette, typography, languages, legal boundary, model naming, and platform order are agreed.
- Repository graphics, visible brand copy, outbound destinations, and desktop identity surfaces are inventoried.
- The canonical brand archive and route-map structure are established.

Exit condition: this architecture, plan, brand README, and route map agree with one another.

### Phase 1 — Select the mark

Concepts 01–03 (Threshold M, Courtyard M, and Folded Workspace) were rejected on 2026-09-24. The supplied open-book/folder reference resets the visual direction.

Concept 04 translates that reference into an original, scalable Maktabi system: a rounded-square container with a three-volume book/file rhythm and a bold, professional wordmark. The raster reference supplies only the high-level composition. The recreated mark uses three identical modules, measured center spacing, consistent margins, and one controlled 10-degree lean. It has been reviewed at large size and at 64, 32, 24, and 16 px in the approved Obsidian/White palette.

Exit condition: complete. Concept 04 geometry and the Obsidian container with White books were approved on 2026-09-24.

### Phase 2 — Finalize the identity system

Complete. The controlling specification is `docs/rebrand/phase-2/PHASE_2_BRAND_ASSET_SYSTEM_SPEC.md`; dependency-ordered work is tracked under `docs/rebrand/phase-2/tickets/`.

- Refine geometry on a documented grid.
- Draw the Latin `Maktabi Agent` wordmark.
- Draw the Arabic `مكتبي` lockup with Tajawal Bold as the construction reference, then convert final lettering to outlines. Keep it as graphic collateral; the final desktop app uses Latin graphic assets only.
- Create a bilingual lockup.
- Establish clear space, minimum size, background rules, and one-color fallbacks.
- Create the Adem family mark and Adem Pro modifier.
- Produce a master asset manifest with version and approval status.

Exit condition: complete. Editable SVG masters are approved, remain legible at the smallest required size, and the manifest is frozen for Phase 3 export generation.

### Phase 3 — Produce Windows and shared exports

- Application icon master and Windows PNG ladder: 16, 24, 32, 48, 64, 128, 256, 512, and 1024 px.
- Multi-resolution `icon.ico`.
- Window/taskbar PNG, tray ICO, installer/uninstaller/header icon, and Preview variant.
- Web favicon and shared UI symbol.
- README/social avatar exports.
- Future macOS and iOS master canvases without claiming a native iOS application exists.

Exit condition: each export has a route-map destination, checksum, dimensions, and approval state.

### Phase 4 — Produce experience graphics

- Startup/loading badge and motion treatment.
- Login/welcome hero using the approved book/workspace geometry.
- Maktabi account and model connection illustration showing Adem and Adem Pro only.
- Completion/ready graphic.
- New-conversation empty state.
- Reusable website/login banner.
- Replace remote ZCode promotional artwork with owned local assets or Maktabi CDN assets.

Instructional screenshots of Terminal, Finder, and Feishu remain only when accurate, licensed, and useful. They are reviewed rather than automatically redrawn.

Exit condition: every graphic works on the near-black theme, has a light-theme treatment where required, and contains no baked-in upstream name or destination.

### Phase 5 — Specify service contracts

This phase starts when the Maktabi platform details are supplied.

- Account authorization and `maktabi://auth/callback` contract.
- Session/token handling and user information.
- Adem/Adem Pro catalogue, entitlements, quotas, and thinking-level API.
- OmniRoute request and streaming contract.
- PayPart purchase, subscription, renewal, cancellation, and entitlement refresh.
- Documentation, support, privacy, terms, status, community, downloads, updates, plugins, and sharing routes.

Exit condition: every destination in the route map is live or the corresponding UI is disabled.

### Phase 6 — Implement the customer-facing rebrand

Implementation order:

1. Add a single shared Maktabi brand module and public asset entry points.
2. Replace startup, welcome, onboarding, empty-state, window, sidebar, About, and web/share identity.
3. Add English, French, and Arabic catalogues and verify RTL layout.
4. Replace desktop product identity, app ID, executable/package name, protocol, shortcuts, and installer metadata.
5. Replace Maktabi-owned links and disable unresolved upstream-dependent actions.
6. Replace the default provider experience with Adem and Adem Pro; move compatible third-party configuration under Advanced Settings.
7. Rename customer-visible theme labels while keeping the black visual character.
8. Add the legal “Based on ZCode” notice and preserve third-party notices.

Each behavior change must first update its focused specification and add the relevant tests or E2E scenario, following repository policy.

### Phase 7 — Verify the Windows release

- Run repository typecheck, lint, formatting check, and changed-architecture check.
- Build the desktop application and Windows installer.
- Test clean install, upgrade, side-by-side Preview install, shortcuts, Start menu, protocol registration, taskbar, tray, About, update behavior, and uninstall.
- Exercise first run in English, French, Arabic, RTL, dark mode, and light mode.
- Test login callback, entitlement loading, Adem selection, thinking levels, logout, offline state, and expired sessions.
- Crawl clickable product links and confirm that each resolves to an approved Maktabi destination.
- Run the residual-brand scan and adjudicate every remaining match.

Exit condition: all acceptance scenarios in the architecture pass and there are no unexplained upstream brand matches in a distributed artifact.

### Phase 8 — Plan internal identifier migration

After the Windows release is stable, write a separate compatibility specification for `@zcode/*`, `.zcode`, `ZCODE_*`, protocol names, telemetry keys, and plugin IDs. Define dual-read/dual-write or aliases where existing user data and ecosystem integrations require them.

## Proposed implementation tickets

| Order | Ticket | Depends on |
| ---: | --- | --- |
| 1 | Approve and finalize Maktabi master logo | Current concepts |
| 2 | Generate the export matrix and asset manifest | 1 |
| 3 | Add shared brand component and theme token specification | 1 |
| 4 | Rebrand Windows package and installer identity | 2 |
| 5 | Rebrand startup, welcome, onboarding, and empty states | 2, 3 |
| 6 | Add French and Arabic/RTL product localization | 3 |
| 7 | Define and implement Maktabi authentication | Server contract |
| 8 | Define and implement Adem/Adem Pro integration | Server contract, 7 |
| 9 | Replace help, community, feedback, docs, and download routes | Live destinations |
| 10 | Replace update, plugin, and share services | Live service contracts |
| 11 | Update legal presentation and release notices | Product owner/legal review |
| 12 | Windows installer and end-to-end rebrand verification | 4–11 |
| 13 | Internal identifier compatibility plan | Stable Windows release |

## Verification commands

Run from the repository root during implementation:

```text
pnpm typecheck
pnpm lint
pnpm fmt:check
pnpm architecture:check --changed
```

Package-specific tests and E2E commands must be taken from the current target package and test files. Do not assume a repository-wide test command exists.

## Residual brand scan

The final audit searches, at minimum, for:

```text
ZCode
zcode
Z.AI
Z.ai
z.ai
zai-org
zcode.z.ai
chat.z.ai
api.z.ai
cdn-zcode.z.ai
dev.zcode.app
zcode://
@zcode/
.zcode
```

Each result receives one disposition: replace, remove, disable pending service, preserve as third-party provider, preserve for compatibility, preserve for legal attribution, or false positive.

## Inputs still expected later

- GitHub organization and repository URL.
- Public support and maintainer email addresses.
- Final Maktabi endpoint and callback contracts.
- PayPart integration details.
- Download, update, marketplace, sharing, documentation, privacy, terms, status, feedback, and community destinations.
- Adem/Adem Pro model IDs, quotas, context limits, and API schema.

These inputs do not block logo selection and master asset production.
