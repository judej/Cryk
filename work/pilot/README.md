# Private pilot work

Use the [mission](mission.md) for scope and approval. The planner owns assignments and the [run record](run.md). Every ticket starts unassigned. A plan request can start with P01. Implementation requires approval of the selected ticket or plan.

The [development plan, revision 1](development-plan.md) maps the design to ticket deliverables, acceptance evidence, and release decisions.

| Ticket | Depends on | State | Owner |
| --- | --- | --- | --- |
| [P01 · One private tenant](issues/P01-identity.md) | None | Plan ready for approval | Unassigned |
| [P02 · A scoped read-only connection](issues/P02-connection.md) | P01 | Waiting for dependencies | Unassigned |
| [P03 · A recoverable Gmail scan](issues/P03-synchronization.md) | P02 | Waiting for dependencies | Unassigned |
| [P04 · Obligations with persistent user corrections](issues/P04-actions.md) | P03 | Waiting for dependencies | Unassigned |
| [P05 · Two private web briefings and urgent notices](issues/P05-briefings.md) | P04 | Waiting for dependencies | Unassigned |
| [P06 · Withdrawal, purge, and restore](issues/P06-withdrawal.md) | P05 | Waiting for dependencies | Unassigned |
| [P07 · Pilot admission and evaluation](issues/P07-pilot-evidence.md) | P06 | Waiting for dependencies | Unassigned |

After approval, the planner records the owner and moves the ticket to In progress. The worker returns evidence for review. The planner marks the ticket Complete after independent acceptance.
