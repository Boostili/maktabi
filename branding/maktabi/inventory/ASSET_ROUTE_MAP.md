# Maktabi Asset, Text, and Link Route Map

Status: repository inventory plus planned routes  
Last scanned: 2026-09-27
Runtime replacement: not started

## How to use this map

This file records every discovered customer-facing brand surface and the future Maktabi source that should own it. A row marked `keep/review` is not automatically replaced. A row marked `blocked` needs a live Maktabi service or a separate compatibility decision.

Status values:

- `concept`: created for selection, not approved.
- `preferred`: selected by the owner as the active direction, still awaiting final geometry or color approval.
- `approved`: confirmed source direction; production derivatives may be created from it.
- `rejected`: retained as design history and prohibited from production use.
- `planned`: future Maktabi asset or change has a defined route.
- `replace`: existing upstream brand surface must change.
- `remove`: upstream product/service surface will not exist in the default Maktabi experience.
- `keep/review`: neutral or third-party material may remain after accuracy and license review.
- `blocked`: destination or contract is still required.
- `legal`: preserve for attribution or license compliance.
- `internal`: customer-invisible compatibility identifier, deferred.

## New concept assets

| Source | Purpose | Status |
| --- | --- | --- |
| `branding/maktabi/source/concepts/maktabi-agent-concept-01-threshold.svg` | Threshold M concept board | rejected |
| `branding/maktabi/source/concepts/maktabi-agent-concept-02-courtyard.svg` | Courtyard M concept board | rejected |
| `branding/maktabi/source/concepts/maktabi-agent-concept-03-folded-workspace.svg` | Folded Workspace concept board | rejected |
| `branding/maktabi/source/concepts/maktabi-agent-concept-04-book-workspace.svg` | Confirmed geometric book/workspace board in the Obsidian/White palette | approved |
| `branding/maktabi/source/concepts/maktabi-agent-concept-04-symbol.svg` | Confirmed isolated transparent-background Concept 04 vector symbol | approved |
| User-supplied `Minimalist Logo with Open Book and Folder.png` | Composition reference only; do not copy, archive as a Maktabi master, or distribute | keep/review |

## Planned master-to-runtime routes

These filenames become authoritative after a logo direction is approved.

| Maktabi master/export | Exact runtime destination | Consumer | Status |
| --- | --- | --- | --- |
| `source/maktabi-agent-mark-primary.svg` | `packages/ui/src/assets/maktabi-agent-mark.svg` | Shared UI brand component | approved master; runtime copy planned |
| `source/maktabi-agent-lockup-latin-horizontal.svg` | `packages/ui/src/assets/maktabi-agent-lockup.svg` | Login, onboarding, About, web | approved master; runtime copy planned |
| `source/maktabi-agent-lockup-ar-horizontal.svg` | No default runtime destination | Approved Arabic graphic collateral and marketing only; the final desktop app ships Latin graphic assets only | planned |
| `source/maktabi-agent-lockup-bilingual.svg` | No default runtime copy; selected banners/docs only | Bilingual collateral; desktop app remains Latin-only | approved |
| `source/maktabi-agent-mark-preview.svg` | Future Preview-specific builder route | Side-by-side Preview identity | approved |
| `source/maktabi-agent-mark-one-color-dark.svg` | Future monochrome system export | Dark one-color fallback | approved |
| `source/maktabi-agent-mark-one-color-light.svg` | Future monochrome system export | Light one-color fallback | approved |
| `source/adem-model-mark.svg` | `packages/ui/src/assets/provider-icons/model-provider-adem.svg` | Default model/provider UI | approved master; runtime copy planned |
| `source/adem-pro-model-mark.svg` | `packages/ui/src/assets/provider-icons/model-provider-adem-pro.svg` | Pro model UI | approved master; runtime copy planned |
| `exports/app/maktabi-agent-empty-state-dark.svg` | `packages/ui/src/assets/maktabi-agent-empty-state-dark.svg` | New-conversation empty state | draft export; visual review pending |
| `exports/app/maktabi-agent-startup-mark.svg` | Shared component or `packages/ui/src/assets/maktabi-agent-startup-mark.svg` | Startup and occupation onboarding | draft export; visual review pending |
| `exports/app/maktabi-agent-onboarding-welcome-dark.svg` | `packages/ui/src/onboarding/assets/maktabi-agent-welcome-dark.svg` | Welcome/login hero | draft export; visual review pending |
| `exports/app/maktabi-agent-onboarding-models-dark.svg` | `packages/ui/src/onboarding/assets/maktabi-agent-models-dark.svg` | Adem connection step | draft export; visual review pending |
| `exports/app/maktabi-agent-onboarding-ready-dark.svg` | `packages/ui/src/onboarding/assets/maktabi-agent-ready-dark.svg` | Completion state | draft export; visual review pending |
| `exports/app/maktabi-agent-banner-dark.svg` | Website/login banner route to be confirmed | Reusable marketing/login banner | draft export; visual review pending |
| `exports/windows/icon-windows.png` | `HARNESS_ROOT/packages/desktop/build/icon_windows.png` | Window/taskbar runtime resource | approved export; runtime copy planned |
| `exports/windows/icon-installer.png` | `HARNESS_ROOT/packages/desktop/build/icon_installer.png` | Installer source preview | approved export; runtime copy planned |
| `exports/windows/icon-installer.ico` | `HARNESS_ROOT/packages/desktop/build/icon_installer.ico` | Installer, uninstaller, NSIS header | approved export; runtime copy planned |
| `exports/windows/icon.ico` | `HARNESS_ROOT/packages/desktop/build/icon.ico` | App/tray and Windows package | approved export; runtime copy planned |
| `exports/windows/icon.png` | `HARNESS_ROOT/packages/desktop/build/icon.png` | Packaged cross-platform resource | approved export; runtime copy planned |
| `exports/windows/icons/16x16.png` | `HARNESS_ROOT/packages/desktop/build/icons/16x16.png` and `HARNESS_ROOT/public/logo/icons/16x16.png` | Package/readme export | approved export; runtime copy planned |
| `exports/windows/icons/24x24.png` | `HARNESS_ROOT/packages/desktop/build/icons/24x24.png` and `HARNESS_ROOT/public/logo/icons/24x24.png` | Package/readme export | approved export; runtime copy planned |
| `exports/windows/icons/32x32.png` | `HARNESS_ROOT/packages/desktop/build/icons/32x32.png` and `HARNESS_ROOT/public/logo/icons/32x32.png` | Package/readme export | approved export; runtime copy planned |
| `exports/windows/icons/48x48.png` | `HARNESS_ROOT/packages/desktop/build/icons/48x48.png` and `HARNESS_ROOT/public/logo/icons/48x48.png` | Package/readme export | approved export; runtime copy planned |
| `exports/windows/icons/64x64.png` | `HARNESS_ROOT/packages/desktop/build/icons/64x64.png` and `HARNESS_ROOT/public/logo/icons/64x64.png` | Package/readme export | approved export; runtime copy planned |
| `exports/windows/icons/128x128.png` | `HARNESS_ROOT/packages/desktop/build/icons/128x128.png` and `HARNESS_ROOT/public/logo/icons/128x128.png` | Package/readme export | approved export; runtime copy planned |
| `exports/windows/icons/256x256.png` | `HARNESS_ROOT/packages/desktop/build/icons/256x256.png` and `HARNESS_ROOT/public/logo/icons/256x256.png` | Package/readme export | approved export; runtime copy planned |
| `exports/windows/icons/512x512.png` | `HARNESS_ROOT/packages/desktop/build/icons/512x512.png` and `HARNESS_ROOT/public/logo/icons/512x512.png` | Package/readme export | approved export; runtime copy planned |
| `exports/windows/icons/1024x1024.png` | `HARNESS_ROOT/packages/desktop/build/icons/1024x1024.png` and `HARNESS_ROOT/public/logo/icons/1024x1024.png` | Package/readme master export | approved export; runtime copy planned |
| `exports/windows/icon-preview.ico` | `HARNESS_ROOT/packages/desktop/build/icon_preview.ico` | Side-by-side Preview identity | approved export; runtime copy planned |
| `exports/web/favicon.ico` | `HARNESS_ROOT/packages/web/public/favicon.ico` | Web/browser tab | approved export; runtime copy planned |
| `exports/web/icon-1024.png` | `HARNESS_ROOT/public/icon_512@2x.png` | Repository/web display and README/avatar | approved export; runtime copy planned |
| `exports/app/icon.icns` | `packages/desktop/build/icon.icns` and `public/logo/icons/icon.icns` | Future macOS package/readme | planned |
| `exports/app/icon.ico` | `public/logo/icons/icon.ico` | Repository/documentation | planned |
| `exports/macos/dmg-background.png` | `packages/desktop/build/dmg_background.png` | Future macOS DMG | planned |
| `exports/macos/dmg-background@2x.png` | `packages/desktop/build/dmg_background@2x.png` | Future Retina DMG | planned |
| `exports/macos/icon-installer.icns` | `packages/desktop/build/icon_installer.icns` | Future DMG volume icon | planned |
| `exports/future-ios/app-icon-master.svg` | No current runtime destination | Future native iOS project | planned |

## Existing graphical assets that carry product identity

| Existing source | Current use | Disposition |
| --- | --- | --- |
| `packages/ui/src/assets/Z.svg` | Dark conversation empty-state artwork | replace with owned Maktabi empty-state art |
| `packages/ui/src/assets/provider-icons/logo-zai.svg` | Sidebar rail, Windows title logo, application shell, OAuth icon | split app identity from provider identity; replace app uses and remove default Z.ai auth use |
| `packages/ui/src/assets/provider-icons/logo-zai-square.svg` | Z.ai square provider logo | remove from default experience; preserve only if later offered explicitly as a third-party provider |
| `packages/ui/src/assets/provider-icons/model-provider-zai.png` | Z.ai model/provider presentation | remove from default experience |
| `packages/ui/src/assets/provider-icons/model-provider-zai-app.png` | Z.ai app/provider presentation | remove from default experience |
| `packages/ui/src/assets/provider-icons/model-provider-start-plan.png` | Z.ai Start/Coding Plan presentation | remove |
| `packages/ui/src/assets/cli-icons/icon-glm.png` | GLM CLI/provider branding | remove from default experience or retain only as explicit third-party provider |
| `packages/ui/src/assets/cli-icons/icon-glm-for-light.png` | GLM monochrome light treatment | same disposition as GLM provider |
| `packages/ui/src/assets/cli-icons/icon-glm-for-dark.png` | GLM monochrome dark treatment | same disposition as GLM provider |
| `packages/desktop/build/icon_windows.png` | Windows window/taskbar icon | replace |
| `packages/desktop/build/icon_installer.png` | Installer source artwork | replace |
| `packages/desktop/build/icon_installer.ico` | Windows installer/uninstaller/header | replace |
| `packages/desktop/build/icon_installer.icns` | macOS installer/DMG icon | replace in later macOS export pass |
| `packages/desktop/build/icon.png` | Packaged app resource | replace |
| `packages/desktop/build/icon.ico` | Windows app and tray source | replace |
| `packages/desktop/build/icon.icns` | macOS application icon | replace in later macOS export pass |
| `packages/desktop/build/icons/*.png` | 16–1024 px application icon ladder | replace from approved master |
| `packages/desktop/build/dmg_background.png` | macOS installation artwork | replace in later macOS pass |
| `packages/desktop/build/dmg_background@2x.png` | Retina macOS installation artwork | replace in later macOS pass |
| `packages/web/public/favicon.ico` | Web favicon | replace |
| `public/logo/icons/icon.ico` | Public/readme Windows icon | replace |
| `public/logo/icons/icon.icns` | Public/readme macOS icon | replace |
| `public/logo/icons/*.png` | Public/readme icon ladder | replace |
| `public/icon_512@2x.png` | Public 1024 px icon | replace |

## Existing code-drawn graphical surfaces

These are assets even though they are implemented as JSX, Canvas, or CSS.

| Source | Surface | Disposition |
| --- | --- | --- |
| `packages/ui/src/components/ui/ZCodeAboutLogo.tsx` | Welcome, onboarding, and About-style logo drawing | replace with a neutral `MaktabiAgentLogo` component consuming the approved master |
| `packages/ui/src/root/RootStartupLoading.tsx` | Startup badge and animated mark | redraw with the selected Maktabi geometry |
| `packages/ui/src/onboarding/OccupationOnboardingVisual.tsx` | First-run brand visual | route to Maktabi startup mark and illustration system |
| `packages/ui/src/onboarding/OnboardingWelcomeView.tsx` | First-run welcome logo and accessible label | replace component and `aria-label` |
| `packages/ui/src/onboarding/onboardingMeshRenderer.ts` | Generated onboarding mesh | retain technique; retune to the two-color Maktabi system after visual approval |
| `packages/ui/src/onboarding/onboardingLogoSweep.css` | Animated onboarding logo border | recolor/refine for the selected mark and reduced-motion behavior |
| `packages/ui/src/v4/ConversationDraftEmptyState.tsx` | Empty-state composition and inline SVG | replace Z art and verify both interface modes |
| `packages/ui/src/WindowsTopLeftLogo.tsx` | Windows title-bar mark | replace app-logo import |
| `packages/ui/src/WorkspaceSidebar/WorkspaceSidebarCollapsedRail.tsx` | Collapsed sidebar mark | replace app-logo import |
| `packages/ui/src/App.tsx` | Shell/fallback app logo | replace app-logo import |
| `packages/ui/src/WelcomeScreen.tsx` | Login/welcome logo and Z.ai choices | use Maktabi identity and Maktabi account flow |
| `packages/desktop/src/main/aboutWindow.ts` | About window layout and inline decorative SVG | route to Maktabi application icon/lockup |

## Instructional and third-party graphics

| Source group | Disposition |
| --- | --- |
| `packages/ui/src/onboarding/assets/terminal.png` | keep/review for accuracy and provenance |
| `packages/ui/src/onboarding/assets/finder.png` | keep/review; macOS-specific and outside the first Windows milestone |
| `packages/ui/src/onboarding/assets/feishu.png` | review carefully; remove if it leads to an upstream/community workflow Maktabi does not ship |
| `packages/ui/src/assets/provider-icons/model-provider-*.{png,svg}` excluding Z.ai/Start Plan | retain as third-party provider marks only where the provider remains available under Advanced Settings; preserve original colors and attribution |
| `packages/ui/src/assets/provider-icons/logo-openrouter.svg`, `logo-moonshoot.svg`, `logo-bigmodel.svg`, `logo-anthropic.svg` | third-party marks; do not recolor into Maktabi branding |
| `packages/ui/src/assets/payment-icons/*` | preserve payment-network marks only when PayPart/payment UI legitimately supports them |
| `packages/ui/src/assets/plugin-icons/*` | keep/review as product capability icons; replace only when provenance or visual consistency fails review |
| `packages/ui/src/assets/document-skill-icons/*` | keep/review as capability art |
| `packages/web/public/material-icons/*` and `packages/desktop/src/renderer/public/material-icons/*` | third-party file-type icon library; exclude from Maktabi logo replacement and preserve its notices |

## Remote and generated artwork routes

| Source | Current destination | Disposition |
| --- | --- | --- |
| `packages/ui/src/v4/featureSuggestedPrompts.ts` | `https://cdn-zcode.z.ai/zcode/official-plugin/assets` | replace with local approved Maktabi assets or a Maktabi-owned CDN after service setup |
| `apps/zcode-cli/packages/bootstrap/src/app/official-plugin-definitions.ts` | Same upstream official-plugin CDN | block public Maktabi marketplace release until replaced or the affected plugin cards are disabled |
| `packages/desktop/src/main/remoteCdn.ts` | `https://cdn-zcode.z.ai` | replace with Maktabi distribution host after contract exists |
| `packages/ui/src/components/ai-elements/persona.tsx` | External Vercel-hosted Rive persona files | license/provenance review; either vendor approved copies or remove from Maktabi-owned brand surfaces |

## Product names and visible text

| Exact source | Visible content | Disposition |
| --- | --- | --- |
| `packages/ui/src/i18n/locales/en-US.ts` | English ZCode/Z.ai product copy across startup, login, About/help, settings, sharing, providers, plugins, errors, resource manager, onboarding, chat, workflows, feedback, and quotas | replace or remove by feature; add French and Arabic peers |
| `packages/ui/src/i18n/locales/zh-CN.ts` | Chinese upstream product copy | remove from Maktabi’s supported first-release language set or retain only if explicitly supported later; it must not remain the fallback for missing Maktabi copy |
| `packages/ui/src/WorkspaceSidebarFooter.tsx` | Fallback product name `ZCode`; theme IDs `zai-dark` and `zai-light` are exposed through labels | show Maktabi; migrate customer-visible labels while treating stored IDs as compatibility data |
| `packages/ui/src/WelcomeScreen.tsx` | `ZCode` accessible label and Z.ai/BigModel login choices | replace with Maktabi account experience |
| `packages/ui/src/onboarding/OnboardingWelcomeView.tsx` | `ZCode` accessible label | replace |
| `packages/web/index.html` | Browser title `ZCode` | replace |
| `packages/web/src/main.tsx` | Sign-in, share, web, and server document titles | replace |
| `packages/web/src/auth/webAuthLocale.ts` | ZCode/Z.AI login copy | replace with Maktabi English/French/Arabic copy |
| `packages/web/src/share/ConversationShareLandingPage.tsx` | ZCode share branding, buttons, labels, and download copy | disable until Maktabi share exists, then replace |
| `packages/desktop/src/main/about.ts` | `ZCode Desktop App`, About title, and copyright | replace with Maktabi Agent and Maktabi copyright; add legal attribution link/entry |
| `packages/desktop/src/main/desktopApplicationMenu.ts` plus UI locale message IDs | About, update, endpoint, diagnostics, feedback, and help labels | replace customer-visible product wording; internal command IDs can remain temporarily |
| `packages/zcode-server-cli/src/**` runtime messages | `ZCode Server` service and error copy | replace when the server is distributed as Maktabi; internal types may remain |
| `apps/zcode-cli/packages/i18n/src/locales/en-US.ts` | CLI/TUI ZCode and Z.AI help/login/runtime copy | replace for the shipped `maktabi` CLI |
| `apps/zcode-cli/packages/i18n/src/locales/zh-CN.ts` | Chinese CLI/TUI upstream copy | same language decision as the desktop Chinese catalogue |
| `apps/zcode-cli/packages/cli/src/login-command.ts` | Browser authorization message naming Z.AI/BigModel | replace with Maktabi account language |
| `apps/zcode-cli/packages/core/src/tool/handlers/webfetch-constants.ts` | Public `ZCode-WebFetch` user agent and `zcode.ai` reference | replace in distributed Maktabi runtime |
| `README.md`, `README.en.md` | Repository name, logos, commands, screenshots, links, and upstream positioning | rewrite after GitHub identity is provided; preserve attribution/license section |
| `NOTICE.md` | Product risk disclosure plus ZCode references | update product description carefully and add “Based on ZCode”; preserve required provenance |

## Desktop and operating-system identity

| Exact source | Current identity | Planned identity/status |
| --- | --- | --- |
| `packages/desktop/scripts/desktop-product-identity.mjs` | `ZCode`, `ZCode Preview`, `dev.zcode.app`, `zcode`, `zcode-preview`, development AUMID `cn.aminer.zcode` | `Maktabi Agent`, `Maktabi Agent Preview`, `space.maktabi.agent`, `maktabi-agent`, `maktabi-agent-preview`; specify development AUMID during implementation |
| `packages/desktop/package.json` | Description, author, product name | replace with Maktabi metadata |
| `packages/desktop/electron-builder.config.js` | Homepage, author, maintainer, product name, scheme, artifacts, icon routes | replace with Maktabi values and `maktabi` scheme after live endpoints/signing identity exist |
| `packages/desktop/build/installer.nsh` | `ZCode` log paths, labels, manifest name, function/macro identifiers | replace user-visible log/detail text and public filenames; internal macro identifiers may remain until installer compatibility is proven |
| `packages/desktop/src/main/desktopOAuthDeepLink.ts` | Hard-coded `zcode` protocol | migrate to `maktabi` with explicit upgrade behavior |
| `packages/desktop/src/main/desktopLinuxDeepLinkRegistration.ts` | `x-scheme-handler/zcode` and default `ZCode` | replace for later Linux release |
| `packages/zcode-cua/broker-helper-constants.js` | ZCode Computer Use names and `dev.zcode.*` bundle IDs | replace before distributing the helper under Maktabi |
| `packages/zcode-server-cli/src/platform/serviceManager.ts` | `com.zhipu.zcode.server` service identity | replace during server packaging migration |
| `.release-it.mjs`, build/release scripts, environment files | ZCode artifact and release naming | inventory again when GitHub/release hosting is supplied |

## Clickable links and network destinations

| Source | Current destination | Maktabi destination/action | Status |
| --- | --- | --- | --- |
| `packages/desktop/electron-builder.config.js` | `https://zcode.z.ai`; `dev@zcode.z.ai` | `https://maktabi.space`; maintainer email TBD | blocked for email |
| `packages/ui/src/lib/productDocs.ts` | `https://zcode.z.ai/docs` | proposed `https://maktabi.space/docs` | blocked until live |
| `packages/web/src/share/ConversationShareLandingPage.tsx` | `https://zcode.z.ai` download and `zcode://share/import` | proposed Maktabi download route and `maktabi://share/import`; disable until service exists | blocked |
| `packages/shared/src/zcodeEndpoint.ts` | `https://zcode.z.ai`, `https://chat.z.ai`, `https://api.z.ai`, upstream OAuth client ID | Maktabi endpoint/auth/business configuration | blocked on server contract |
| `packages/services/src/oauth/providers/zaiProviderConfig.ts` | Z.ai authorize/token/userinfo/business login | Maktabi OAuth adapter | remove/replace |
| `packages/services/src/oauth/providers/bigmodelProviderConfig.ts` | ZCode token exchange | remove from default experience |
| `packages/ui/src/settings/model-provider-section/constants.ts` | Z.ai subscription purchase page | PayPart/Maktabi plan route | blocked on payment contract |
| `packages/shared/src/model-provider-family.ts` | Z.ai team plan management | Maktabi account/plan route | blocked |
| `config/provider/zcode-builtin.json` | Z.ai API key, Anthropic/OpenAI-compatible endpoints, ZCode plans | replace built-in first-party catalogue with Adem/Adem Pro; retain user-configurable third-party providers separately | blocked on model schema |
| `packages/shared/src/plugin-marketplaces.ts` | ZCode official plugin CDN and marketplace ID | Maktabi marketplace or disabled store | blocked |
| `config/default.json` | Zhipu Feishu feedback, Feishu community, upstream Discord | Maktabi support/community destinations | blocked |
| `packages/ui/src/v4/featureSuggestedPrompts.ts` | ZCode official-plugin asset CDN | local/Maktabi-owned assets | replace |
| `packages/desktop/src/main/remoteCdn.ts` | ZCode CDN | Maktabi release CDN | blocked |
| `apps/zcode-cli/packages/adapters/src/model/official-coding-plan-gateway.ts` | Z.ai provider and ZCode gateway | OmniRoute-backed Maktabi model service | blocked |
| `apps/zcode-cli/packages/adapters/src/auth/coding-plan-api-key.ts` | `https://api.z.ai` | Maktabi session/entitlement contract | remove/replace |
| `apps/zcode-cli/packages/adapters/src/auth/cli-oauth.ts` | ZCode OAuth base | Maktabi authorization base | blocked |
| Repository badges and links in `README.md` and `README.en.md` | `zai-org/ZCode` and upstream destinations | Maktabi GitHub organization/repository TBD | blocked |

## Legal and provenance routes

| Source | Rule | Status |
| --- | --- | --- |
| `LICENSE` | Preserve Apache-2.0 license text | legal |
| `NOTICE.md` | Preserve required upstream notices; update product-specific prose carefully and add “Based on ZCode” | legal |
| `THIRD-PARTY-NOTICES.md` | Preserve and regenerate when dependencies/assets change | legal |
| Provider logo source metadata under `packages/ui/src/assets/provider-icons/model-provider-logo-sources.json` | Preserve provenance for third-party marks that remain | legal |
| Material-icon library and redistributed fonts/binaries | Preserve applicable notices and licenses | legal |

## Deferred compatibility identifiers

These are deliberately tracked so they cannot be mistaken for forgotten branding:

| Pattern | Examples | Status |
| --- | --- | --- |
| Package scope | `@zcode/shared`, `@zcode/ui`, other `@zcode/*` imports | internal |
| Code symbols | `ZCodeAgentService`, `getZCodeCopy`, protocol types | internal |
| User/project storage | `~/.zcode`, `.zcode/workflows`, `.zcode-plugin` | internal; separate migration required |
| Environment variables | `ZCODE_ENV`, `ZCODE_STORAGE_DIR`, endpoint variables | internal; alias plan required |
| Protocol metadata | `application/vnd.zcode.*`, `com.zcode/*`, RPC channel names | internal; compatibility plan required |
| Telemetry keys | `zcode.execution.*` | internal; privacy/schema migration required |
| Theme persistence | `zcode-theme`, values `zai-dark`/`zai-light` | internal stored IDs; visible labels change first |

## Final audit rule

Before release, scan source and unpacked artifacts for all upstream identifiers. Every match must point to a row in this map or be filed as a defect. The audit includes images with baked-in text, SVG metadata, HTML titles, ARIA labels, installer resources, executable metadata, shortcuts, protocol registrations, network requests, logs shown to users, and packaged notices.
