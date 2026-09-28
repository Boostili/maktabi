# MKT-307 — Rebrand the CLI and public runtime identity

- Status: Blocked
- Milestone: CLI/public runtime
- Depends on: focused CLI compatibility specification

## Outcome

Ship the user-facing command as `maktabi` and replace public CLI/TUI/server copy without breaking persisted data or internal protocol compatibility.

## Harness scope

- `HARNESS_ROOT/apps/zcode-cli/`
- `HARNESS_ROOT/packages/zcode-server-cli/`
- Public user-agent strings such as `ZCode-WebFetch`.
- Help, login, errors, prompts, binary/package metadata, and documentation.

## Rules

- Do not mechanically rename `@zcode/*`, protocol types, `.zcode`, or `ZCODE_*`.
- Specify command aliases, data-directory behavior, environment aliases, and rollback first.
- Public network metadata identifies Maktabi truthfully.

## Acceptance

- `maktabi --help`, login, model use, errors, and public server messages contain approved identity.
- Any temporary `zcode` command alias is documented and tested.
- Existing compatible user data remains readable.
- No public request advertises a false upstream product identity unless preserved by an explicit compatibility requirement.
