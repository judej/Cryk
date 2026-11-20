# Coding prompts

Use the repository root as the working directory. Replace the ticket ID or symptom with the actual task.

| Task | Prompt to send |
| --- | --- |
| Design the first change | Use the [planner](planner.md) for P01. Show how a synthetic user gets a tenant-scoped response. Identify the evidence required before implementation. |
| Implement an approved ticket | Implement P01 with the [worker](worker.md). Use the approved plan. Record the checks and request independent review. |
| Review a change | Use the [reviewer](reviewer.md) for P01. Check the approved criteria against the current change. Report findings with file locations. |
| Investigate slow synchronization | Use the [diagnosis prompt](diagnosis.md). A synthetic mailbox takes too long to catch up. Measure source lag, analysis backlog, and due-item latency separately. |
| Resume interrupted work | Read the ticket and run record. Check the current owner, edits, and last passing check. Resume independent work within the approved scope. |
| Prepare a release decision | Compare the integrated revision with the [acceptance guide](../../docs/acceptance/README.md). Report measured results and missing evidence for each gate. |
