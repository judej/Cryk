# P06 · Withdrawal, purge, and restore

**Dependencies:** P05.

**Design sections:** Content handling and retention · Provider operations and recovery in the [version 3 design](../../../docs/design/service-v3.md).

**Expected ownership:** Connection admission, storage, keys, and operations. The planner records exact paths before assignment.

Prove that access withdrawal survives queued work, in-flight requests, and backup restoration.

## Acceptance criteria

- [ ] P06-1. Serialize admission and disconnect on the same connection. Hide dependent results immediately. Discard results from an obsolete epoch.
- [ ] P06-2. Distinguish pause, disconnect, and account deletion. Prove the live purge and backup expiry limits from the design.
- [ ] P06-3. Restore with dispatch closed. Replay the independent deletion and revocation ledger. Exercise key rotation and missing authority records.
- [ ] P06-4. Trace synthetic markers across durable destinations. Record actual restore time and lost updates.

## Evidence

Record the approved revision, reviewed paths, commands, results, independent review, and remaining human decisions here.
