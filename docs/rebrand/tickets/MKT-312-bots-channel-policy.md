# MKT-312 — Rebrand bots and decide Algerian-market channel support

- Status: Blocked
- Milestone: Bot and remote-control journey
- Blocker: product, privacy, and support decision for each channel

## Outcome

Classify the new v3.14.3 bot/remote-control surfaces so Maktabi exposes only supported channels with truthful product copy and safe public protocol names.

## Harness scope

- `HARNESS_ROOT/packages/ui/src/BotsDialog.tsx`
- `HARNESS_ROOT/packages/ui/src/BotsDialog/`
- `HARNESS_ROOT/packages/ui/src/botsUi.ts`
- `HARNESS_ROOT/packages/ui/src/WebRemoteControlDialog.tsx`
- `HARNESS_ROOT/packages/ui/src/assets/channel-icons/`
- `HARNESS_ROOT/packages/services/src/bots/`
- `HARNESS_ROOT/packages/shared/src/bots.ts`

## Decisions required

For Telegram, Discord, Feishu/Lark, Weixin, WeCom, DingTalk, and generic webhooks: ship, hide, or future. Define credential handling, data region/privacy disclosure, support level, and setup documentation. Review `x-zcode-bot-secret`, `zcode.bot.*`, and `node-sdk/zcode` separately as compatibility/public protocol identifiers.

## Acceptance

- Unsupported channels are absent or explicitly unavailable; they do not create dead-end Maktabi flows.
- Shipped third-party icons retain provenance and are not recolored as Maktabi assets.
- All visible ZCode copy in bot setup/runtime states is replaced.
- Any renamed webhook header or event type has a compatibility and security migration test.
- No Feishu/Zhipu route is retained merely because it existed upstream.
