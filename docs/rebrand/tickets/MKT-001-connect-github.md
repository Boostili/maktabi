# MKT-001 — Connect the Maktabi GitHub repository

- Status: In-progress
- Milestone: Repository setup
- Blocker: GitHub visibility and repository settings; the approved destination is `Boostili/maktabi`, intended public, default branch `main`

## Outcome

Connect the local `maktabi/` repository to its approved GitHub home without changing the ZCode upstream remote owned by `zcode-harness/`.

## Scope

- Create or identify the Maktabi GitHub repository.
- Add it as `origin` for the Maktabi repository only.
- Publish the existing brand, specification, ADR, inventory, and ticket history.
- Add repository description, website `https://maktabi.space`, topics, issue/PR settings, and branch protection.
- Replace README badge and source links only after the final URL exists.
- Record how cross-repository implementation changes link Maktabi tickets to harness pull requests.

## Out of scope

- Repointing `HARNESS_ROOT` away from `https://github.com/zai-org/ZCode.git` before a deliberate fork strategy is approved.
- Publishing secrets, service URLs, or private contracts.

## Acceptance

- `git remote -v` in `maktabi/` shows only the approved destination.
- `git remote -v` in `zcode-harness/` still shows the intended harness upstream or later approved fork.
- The default branch and branch rules are documented.
- Public metadata uses Maktabi Agent and `maktabi.space`.
- No upstream issue, discussion, social, or sponsor link is presented as Maktabi-owned.

## Progress evidence

Updated 2026-09-28: the connected GitHub account is `Boostili`, and `Boostili/maktabi` now exists with `main` as its default branch. The local history, brand sources, inventories, tickets, Windows exports, and MKT-102 experience graphics are published at commit `f1c62954973d62d35621e26c1d4fa646b9dc20ed`; the local repository has `origin=https://github.com/Boostili/maktabi.git`. The connected GitHub actions do not expose repository visibility, description, website, topics, issue/PR settings, or branch-protection writes. GitHub currently reports the repository as private, so the remaining handoff is to set it public and apply the documented metadata/rules in GitHub settings.
