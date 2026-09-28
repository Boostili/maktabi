# Maktabi Product Context

## Purpose

This glossary defines the stable product language and ownership boundaries for the Maktabi rebrand. Implementation details belong in focused specifications and tickets.

## Core terms

### Maktabi

The umbrella brand and owner of the customer experience at `maktabi.space`.

### Maktabi Agent

The Windows-first desktop harness product. Its first shipped capability is coding assistance, while its identity is intentionally suitable for broader professional work.

### Maktabi Agent Preview

The separately installable pre-release channel. It must remain distinguishable from production in its icon, application identity, shortcuts, update channel, and data boundary.

### Harness

The application source derived from ZCode and maintained in the sibling `zcode-harness/` repository. It is the only working copy of the application.

### Brand repository

This `maktabi/` repository. It owns editable masters, specifications, decisions, inventories, and tickets; it does not own a duplicate of the harness source.

### Brand master

An editable, approved source asset under `branding/maktabi/source/`. Runtime packages consume exports, never the master itself as an accidental dependency.

### Runtime export

A generated or approved derivative copied into a specific harness path for packaging or UI consumption. Every runtime export must have a route-map row.

### Route map

The inventory in `branding/maktabi/inventory/ASSET_ROUTE_MAP.md` that connects each brand master or upstream surface to its exact owner, destination, disposition, and blocker.

### Customer-facing identity

Names, images, icons, text, links, protocols, metadata, and network destinations a user can see or invoke while installing, launching, using, updating, sharing, or getting help.

### Compatibility identity

Existing internal identifiers such as `@zcode/*`, `.zcode`, `ZCODE_*`, persisted theme values, RPC names, and protocol content types. These are not evidence of a failed visual rebrand when they remain invisible and are explicitly classified.

### Maktabi account

The future Maktabi-owned authentication and entitlement experience. Its endpoint and token contracts are external inputs and must not be guessed.

### Adem

The standard Maktabi model family with Low and Moderate thinking levels.

### Adem Pro

The advanced Maktabi model family with Low, Moderate, High, and Max thinking levels.

### OmniRoute

The server-side routing implementation behind the Adem family. It is not a login option, model brand, or first-run provider name.

### PayPart

The future payment gateway for Maktabi purchases and entitlement changes. Integration waits for an approved contract.

### External blocker

A ticket that cannot be implemented truthfully until the owner supplies a destination, credential boundary, service contract, signing identity, or policy choice. Blocked UI must be disabled or hidden rather than pointed at upstream services.

### Based on ZCode

The approved legal attribution phrase. It belongs in legal notices and provenance surfaces, not ordinary product chrome or marketing.

## Ownership rules

- The Maktabi repository owns product truth, brand truth, ticket state, and source artwork.
- The harness repository owns executable behavior, UI integrations, packaging, and tests.
- Maktabi services own authentication, entitlements, models, payments, updates, sharing, documentation, support, and public downloads.
- Third-party channel and provider marks remain third-party assets and keep their own provenance.
- Windows is the only actionable release platform in the current graph; macOS and iOS remain future backlog.

## Language rules

- Supported first-release languages: English, French, and Modern Standard Arabic.
- Arabic presentation supports RTL.
- Darija is not part of the first release.
- Latin brand typography uses Manrope; Arabic graphic lockups use Tajawal Bold as the construction reference. Arabic UI copy may use its own approved UI font specification.

## Visual rules

- Brand colors are Obsidian `#09090B` and White `#FFFFFF` only.
- The product keeps a near-black default appearance.
- The approved symbol is a rounded Obsidian square with three identical White book/file modules; the first leans 10 degrees and the other two remain upright.
- Rejected concepts remain design history and are not production sources.
