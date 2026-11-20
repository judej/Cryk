# P01 · One private tenant

**Dependencies:** None.

**Design sections:** Identity and permission in the [version 3 design](../../../docs/design/service-v3.md).

**Expected ownership:** API, initial package metadata, migrations, and storage. The planner records exact paths before assignment.

Build the first authenticated API path with a synthetic identity and a tenant-owned record. Establish the role and test infrastructure.

## Acceptance criteria

- [ ] P01-1. Map a verified issuer and subject to the tenant. Cover sign-in, CSRF, session checks, and the distinction between logout and grant revocation.
- [ ] P01-2. Through the API and the actual PostgreSQL runtime roles, prove that a second tenant cannot read or change the record.
- [ ] P01-3. Publish the first versioned API contract. Record reproducible local commands for checks.

## Evidence

Record the approved revision, reviewed paths, commands, results, independent review, and remaining human decisions here.
