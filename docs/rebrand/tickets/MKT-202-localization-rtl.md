# MKT-202 — Add English, French, Arabic, and RTL product coverage

- Status: Ready after focused spec
- Milestone: Localization

## Outcome

Make every supported customer-facing Maktabi journey usable in English, French, and Modern Standard Arabic, with correct RTL behavior.

## Harness scope

- `HARNESS_ROOT/packages/ui/src/i18n/`
- `HARNESS_ROOT/packages/web/src/auth/webAuthLocale.ts`
- `HARNESS_ROOT/apps/zcode-cli/packages/i18n/src/locales/`
- Document titles, ARIA labels, installer-visible strings, and error/help text.

## Rules

- No Darija in the first release.
- Arabic UI copy uses Noto Sans Arabic and logical layout properties; Arabic graphic lockups are separate Tajawal Bold collateral and are not imported by the desktop app.
- Chinese upstream catalogues are not a silent fallback for Maktabi copy.
- Third-party product names remain accurate; Maktabi product names are translated only where the approved language system requires it.

## Acceptance

- Locale parity checks report no missing Maktabi keys across the three catalogues.
- First run, login, model selection, settings, help, errors, bots, and About are exercised in RTL.
- Product names, ARIA labels, and window/document titles contain no unintended upstream brand.
- Screens remain usable at Windows text scaling and narrow desktop widths.
