# P2-03 — Finalize Arabic Wordmark and Lockup

Status: complete
Blocked by: P2-01

## Objective

Create an Arabic `مكتبي` lockup that is native to RTL composition and visually related to the Latin identity.

## Deliverables

- Review-only Tajawal Bold text construction source.
- Outlined `branding/maktabi/source/maktabi-agent-lockup-ar-horizontal.svg`.
- RTL proof on light and near-black fields.

## Current work

- Added the review-only Tajawal Bold text construction source.
- Added the outlined master generated from the shaped `مكتبي` glyph run; the wordmark is on the left, the symbol is on the right, and the symbol remains unmirrored.
- Added an RTL proof board with full-size and `120 px` checks on light and near-black fields.
- Replaced the construction reference with Tajawal Bold from Google Fonts.
- Manifest entry is `approved`; this is graphic collateral only and no runtime package was changed.

## Rules

- Use Tajawal Bold as the construction reference.
- Shape the complete Arabic word before outline conversion.
- Do not mirror the symbol or force Arabic lettering to the Latin width.
- Place the Arabic wordmark on the left and the symbol on the right.
- No Darija copy is introduced.

## Acceptance

- Arabic reading order and joining are correct.
- The approved production SVG contains no `<text>` node.
- Clear space equals at least one `18-unit` module.
- A fluent Arabic reviewer approves the final outlined form before manifest status becomes `approved`.

## Completion evidence

Approved 2026-09-27 after switching to Tajawal Bold, correcting the RTL composition so the wordmark sits left of the symbol, adding a protected text-reference gap, and moving the outlined glyph run upward so the final letter dots are not clipped. The Arabic and bilingual marks remain collateral-only; the desktop app uses Latin graphic assets.
