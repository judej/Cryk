# Service package

The four runtime roles share one Python codebase. Each process uses its own network policy, database role, and key permissions. Python package boundaries describe ownership. Deployment and database controls enforce it.

| Package | Responsibility |
| --- | --- |
| `api/` | FastAPI, verified OIDC identity, tenant-scoped results, local action commands, private briefing and preview responses |
| `scheduler/` | Poll times, due work, admission, attempt binding, and job dispatch using control fields |
| `connector/` | Grant and epoch checks, credential decryption, Gmail reads, scoped transient previews |
| `analysis/` | Scoped source requests, approved model disclosure, classification, and permitted derived results |
| `domain/` | Action identity, evidence, corrections, deadlines, coverage, and briefing rules |
| `storage/` | SQLAlchemy, psycopg, tenant constraints, role-scoped queries, and transactional Procrastinate enqueue |

Keep runtime-specific dependencies inside their boundary. Release 1 has no provider mutation operation. The private web view uses the authenticated API. Initial tickets select the smallest client that satisfies the pilot.

The first implementation ticket owns dependency pins, package metadata, and the first runnable entry point.
