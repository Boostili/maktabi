# ADR 0001: Separate the Maktabi product repository from the application harness

- Status: Accepted
- Date: 2026-09-24

## Context

The application is a full ZCode-derived Git repository, while the rebrand work also needs stable brand masters, product specifications, route inventories, and tickets. Keeping two application copies would create path ambiguity, missed changes, and avoidable merge errors. Putting all planning assets inside the upstream-derived repository would mix Maktabi product truth with a codebase that still needs to receive upstream changes during the rebrand.

## Decision

Use two sibling repositories under the workspace root:

- `zcode-harness/` is the single working application repository and retains the ZCode Git history.
- `maktabi/` is the separate brand, specification, inventory, ADR, and ticket repository.

The Maktabi repository must never contain a duplicate application checkout. Documentation uses `HARNESS_ROOT` to mean `../zcode-harness`. Runtime edits happen only through tickets and only inside the harness. The Maktabi Git remote is intentionally absent until the approved GitHub organization and repository are supplied.

## Consequences

- There is one authoritative application tree, reducing duplicate-change and wrong-folder errors.
- Brand masters and plans can evolve without polluting application history before implementation begins.
- Cross-repository tickets must name exact `HARNESS_ROOT/...` destinations.
- A coordinated change may touch both repositories and therefore needs two status checks and, later, two review links.
- The old top-level checkout remains temporarily as a safety copy until the user opens the two-folder workspace and explicitly approves cleanup; it is not a second working target.

## Rejected alternatives

- Two application repositories: rejected because changes could diverge or land in the wrong copy.
- Put Maktabi planning files inside the harness: rejected because it obscures the boundary between upstream-derived code and Maktabi product ownership.
- Move the active checkout destructively in one step: rejected because it would invalidate the current workspace and makes recovery harder.

## Update

- 2026-09-25: The workspace moved to `D:\Zai01`. The old top-level ZCode checkout and its duplicate root `branding/` and `docs/` copies were removed after verifying the checkout was clean and synced with `origin/main` (`29628c9`) and that the duplicates were byte-identical to the `maktabi/` copies. The two-folder layout is now authoritative: `D:\Zai01\zcode-harness` and `D:\Zai01\maktabi`.
