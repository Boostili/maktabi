# MKT-302 — Rebrand launch, taskbar, tray, shell, and About

- Status: Blocked
- Milestone: Core desktop journey
- Depends on: MKT-201

## Outcome

From process start through the normal app shell, every app-owned visual and accessible product reference presents Maktabi Agent.

## Harness scope

- `HARNESS_ROOT/packages/ui/src/root/RootStartupLoading.tsx`
- `HARNESS_ROOT/packages/ui/src/WindowsTopLeftLogo.tsx`
- `HARNESS_ROOT/packages/ui/src/WorkspaceSidebar/WorkspaceSidebarCollapsedRail.tsx`
- `HARNESS_ROOT/packages/ui/src/App.tsx`
- `HARNESS_ROOT/packages/ui/src/components/ui/ZCodeAboutLogo.tsx`
- `HARNESS_ROOT/packages/desktop/src/main/aboutWindow.ts`
- `HARNESS_ROOT/packages/desktop/src/main/about.ts`
- Window titles, tray labels, menu labels, and user-facing diagnostics.

## Acceptance

- Startup, shell, title bar, taskbar, tray, menus, and About use the shared Maktabi module.
- There is no independent inline upstream logo drawing.
- Accessible names and visible diagnostic copy use Maktabi Agent.
- Light mode remains functional, while near-black is the reference presentation.
