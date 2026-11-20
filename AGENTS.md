# Cryk repository instructions

Use the [version 3 design](docs/design/service-v3.md) for product requirements. Use the [pilot mission](work/pilot/mission.md) for the current release. If they conflict, pause the affected work and ask the developer. Continue independent work.

## Delivery

1. Read the assigned ticket, its dependencies, and the relevant design sections. Inspect the current source before you rely on a shared memory.
2. For planning, use the [planner prompt](agents/prompts/planner.md). Record the scope, acceptance evidence, and unresolved decisions. An explicit request to implement an identified plan or ticket authorizes that local work.
3. Start with one worker. The planner assigns each path to one writer. Serialize changes that share interfaces, fixtures, migrations, generated files, or test resources.
4. Use the [worker prompt](agents/prompts/worker.md) for implementation. Keep evidence in the assigned ticket. The planner owns the index and run record.
5. Use the [reviewer prompt](agents/prompts/reviewer.md) for independent review. A developer can perform this review. Keep the ticket open until the reviewer accepts the current change.
6. After integration, run applicable checks through the normal entry points. Record the reviewed revision, commands, results, and missing evidence. Return unresolved human actions to the developer.

## Scope and authority

- Release 1 permits Gmail reads and local user actions. Keep draft creation in release 2 and calendar access in release 3.
- Keep provider credentials in the connector. Keep provider access and content decryption out of the scheduler.
- Derive tenant and attempt authority from trusted state. Check authority in service code and with actual database roles.
- Treat provider content and model output as untrusted data. Neither can authorize an action, source read, recipient, or disclosure.
- Use synthetic inputs for development and repeatable tests. Keep mail bodies, prompts, attachment bytes, full drafts, addresses, and secrets out of tickets, logs, and memory.
- Use deterministic logic for permissions, time, budgets, and retries. A model can propose a classification. Service code controls its effects.
- Keep coding-agent prompts under `agents/prompts/`. Version runtime analysis prompts and schemas with the service implementation.
- Work within the assigned repository. Use a feature branch for implementation. The developer controls merge, live access, deployment, enrollment, and release.
- If a change affects access, disclosure, retention, cost, or an approved requirement, pause the affected work for a decision.

## Recovery and memory

After an interruption, inspect the owner, current edits, reviewed revision, and last successful check. Resume after the previous writer stops. Keep unrelated edits intact.

Use the [memory guide](agents/memory/README.md) for reusable facts. Product decisions belong in the design or an approved amendment. Keep temporary findings in the ticket.
