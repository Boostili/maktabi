# MKT-303 — Rebrand first run, welcome, and onboarding

- Status: Blocked
- Milestone: First-run journey
- Depends on: MKT-102, MKT-201, MKT-202

## Outcome

Deliver a complete first-run experience using Maktabi-owned visuals and Maktabi destinations in all three supported languages.

## Harness scope

- `HARNESS_ROOT/packages/ui/src/WelcomeScreen.tsx`
- `HARNESS_ROOT/packages/ui/src/onboarding/OnboardingWelcomeView.tsx`
- `HARNESS_ROOT/packages/ui/src/onboarding/OccupationOnboardingVisual.tsx`
- `HARNESS_ROOT/packages/ui/src/onboarding/onboardingMeshRenderer.ts`
- `HARNESS_ROOT/packages/ui/src/onboarding/onboardingLogoSweep.css`
- Instructional screenshots in `HARNESS_ROOT/packages/ui/src/onboarding/assets/`.

## Rules

- Remove Z.ai/BigModel as default login choices; connect only through MKT-304.
- Review Terminal/Finder/Feishu screenshots for Windows relevance, accuracy, and license; do not redraw them automatically.
- Honor reduced motion.
- No baked-in language text inside art.

## Acceptance

- A clean profile completes first run in English, French, and Arabic/RTL.
- Every logo, label, destination, and accessible name is owned or explicitly third-party.
- Offline and unavailable-account states do not send users upstream.
