# P03 · A recoverable Gmail scan

**Dependencies:** P02.

**Design sections:** Synchronization and job execution · Provider operations and recovery in the [version 3 design](../../../docs/design/service-v3.md).

**Expected ownership:** Scheduler, connector reads, checkpoints, and queue integration. The planner records exact paths before assignment.

Read the declared scope including Sent mail. Recover from interruption without losing or duplicating admitted work.

## Acceptance criteria

- [ ] P03-1. Start with five-minute polling, spread polls across accounts, and allow one active synchronization and one pending pass per connection.
- [ ] P03-2. Commit references, pending analysis, and the page cursor on one physical PostgreSQL connection. Prove rollback through the application entry point.
- [ ] P03-3. Crash on the last page, resume, and reconcile changes during the initial scan. On an expired cursor, show incomplete coverage during the bounded rescan.
- [ ] P03-4. Reject stale attempt results. Report reconnection, source lag, and backlog separately.

## Evidence

Record the approved revision, reviewed paths, commands, results, independent review, and remaining human decisions here.
