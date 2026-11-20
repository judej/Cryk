# P02 · A scoped read-only connection

**Dependencies:** P01.

**Design sections:** Identity and permission · Content handling and retention in the [version 3 design](../../../docs/design/service-v3.md).

**Expected ownership:** Connector, consent API, keys, and connection records. The planner records exact paths before assignment.

Bind one Gmail grant to the signed-in tenant. Use synthetic provider responses during development.

## Acceptance criteria

- [ ] P02-1. Record purpose, granted scopes, stable account ID, grant ID, policy version, and epoch. Require a decision before replacing a mailbox.
- [ ] P02-2. Separate credential and derived-content key access. The scheduler cannot decrypt content. The analysis worker cannot decrypt provider credentials.
- [ ] P02-3. Bind every source request to a trusted attempt or authorized preview. Reject stale epochs, incorrect audiences, and attempts to widen scope.

## Evidence

Record the approved revision, reviewed paths, commands, results, independent review, and remaining human decisions here.
