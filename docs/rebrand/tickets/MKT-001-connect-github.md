# MKT-001 — Connect the Maktabi GitHub repository

- Status: In-progress
- Milestone: Repository setup
- Blocker: repository creation/publish access; the approved destination is confirmed as `Boostili/maktabi`, public, default branch `main`

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

Confirmed 2026-09-27: the connected GitHub account is `Boostili`, with no organization required for the approved personal repository destination. `Boostili/maktabi` is not present yet. The connector can inspect repositories but does not expose repository creation; the browser fallback is signed out. Create the empty public repository with `main` as its default branch, then this ticket can add `origin`, publish the local history, and apply the documented metadata and branch rules.
