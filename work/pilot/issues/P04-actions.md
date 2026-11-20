# P04 · Obligations with persistent user corrections

**Dependencies:** P03.

**Design sections:** Information model and user behavior · API and operations · Content handling and retention in the [version 3 design](../../../docs/design/service-v3.md).

**Expected ownership:** Domain, analysis, action storage, and action commands. The planner records exact paths before assignment.

Convert scoped evidence into Decide, Reply, Wait, or Nothing. Keep each obligation distinct.

## Acceptance criteria

- [ ] P04-1. Use a synthetic thread with a price and a delivery date. Close only the price action when a later message supplies it.
- [ ] P04-2. Keep stable action IDs across replay. Preserve user corrections, surface ambiguous matches, and leave inaccessible obligations unresolved.
- [ ] P04-3. Support complete, ignore, reopen, snooze, and version-checked undo. Bind retry keys to caller, target, operation, and fingerprint.
- [ ] P04-4. Enforce authorized processor routes and cost reservations before disclosure. Keep raw content in memory. Persist permitted structured facts only.

## Evidence

Record the approved revision, reviewed paths, commands, results, independent review, and remaining human decisions here.
