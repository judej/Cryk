# Test evidence

| Area | Required evidence |
| --- | --- |
| Domain | Stable action identity, independent obligations, correction preservation, date-only deadlines, repeated and skipped local times |
| Database integration | Actual PostgreSQL runtime roles, tenant isolation, stale-attempt rejection, business change and job rollback on one physical connection |
| Connector | Synthetic Gmail pages, Sent coverage, expired cursors, reconnection, grant withdrawal, and no duplicate work after a crash |
| Privacy | Synthetic marker absent from jobs, records, telemetry, temporary files, caches, and other durable destinations |
| User path | Private sign-in, coverage-first briefing, source access, correction, urgent web notice, and next-sign-in visibility |
| Recovery | Restore with dispatch closed, separate ledger replay, key rotation, recovery time, and lost updates |

Place executable tests beside the corresponding area as each ticket lands. Use synthetic fixtures. Run integration checks through application entry points. Mocks cannot establish PostgreSQL permissions or queue atomicity.
