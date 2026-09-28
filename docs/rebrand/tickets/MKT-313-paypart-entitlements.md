# MKT-313 — Integrate PayPart and entitlement refresh

- Status: Blocked
- Milestone: Purchase journey
- Depends on: MKT-304
- Blocker: PayPart checkout, webhook, subscription, cancellation, and entitlement contracts

## Outcome

Replace Z.ai plan purchase and management routes with the Maktabi/PayPart lifecycle.

## Harness scope

- Subscription and plan surfaces in `HARNESS_ROOT/packages/ui/`.
- Current purchase/management destinations in model-provider constants and shared provider-family configuration.
- Account entitlement refresh after purchase, renewal, downgrade, cancellation, refund, and expiry.

## Rules

- Payment processing happens on approved Maktabi/PayPart web surfaces; the desktop app does not handle raw payment credentials.
- Entitlements come from the Maktabi account service, not from optimistic local payment state.
- Remove Z.ai Coding Plan/Start Plan branding and routes.

## Acceptance

- Purchase return, delayed webhook, cancellation, expired session, failed payment, and entitlement refresh scenarios are tested.
- UI never unlocks Adem Pro solely from a browser return parameter.
- All payment-network logos shown are actually supported and retain their legal presentation.
