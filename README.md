# Cryk

Cryk helps a private user answer two questions from mail. What do I owe someone? What am I waiting for?

Release 1 covers one Gmail account, two daily web briefings, local action corrections, and urgent notices in the web app. The repository currently contains the design, package boundaries, work plan, and coding prompts. Service implementation starts with the first ticket.

## Start here

1. Read the [version 3 design](docs/design/service-v3.md) for product behavior and release conditions.
2. Read the [repository instructions](AGENTS.md) for the delivery procedure.
3. Choose an open [pilot ticket](work/pilot/README.md).
4. Use a [task prompt](agents/prompts/README.md) to plan, implement, diagnose, or review the work.

## Repository map

| Path | Purpose |
| --- | --- |
| [src/cryk](src/cryk/README.md) | One Python package with four runtime roles and shared domain and storage code |
| [migrations](migrations/README.md) | Alembic revisions, database roles, and database policies |
| [tests](tests/README.md) | Synthetic examples and behavioral, isolation, and recovery checks |
| [ops](ops/README.md) | Deployment boundaries and operator evidence |
| [work/pilot](work/pilot/README.md) | Mission, dependencies, ticket ownership, and run record |
| [docs/acceptance](docs/acceptance/README.md) | Release evidence and the human decision |
| [agents/memory](agents/memory/README.md) | Verified facts for future tasks |

The repository contains no configured accounts, running services, or pilot approvals.
