# Pilot acceptance

For each gate, record the reviewed revision, environment, date, owner, sample size, target, actual result, and evidence location. Keep unknown or unmeasured results open.

| Gate | Evidence |
| --- | --- |
| Admission | Account eligibility, scopes and source window, published retention, named operator, processor route and expiry, verified tenant and audience isolation |
| Detection and usefulness | Independent sample of the declared scope, missed obligations, false closures, useful alerts, and net time saved after user corrections |
| Due work | At least 95 percent of known due actions appear within ten minutes while the service is available. Record backlog, provider lag, and notice failure separately. |
| Recovery | Restore read access within four hours with at most 15 minutes of lost application updates. Show that deletions and revocations survive. |
| Privacy | Demonstrate immediate withdrawal of derived access and absence of synthetic message content from durable destinations. |
| Promotion | Keep tuning and evaluation samples separate. Run a read-only shadow period. Record the release owner's decision and rollback conditions. |

The design proposes the numeric targets above. The owner records the adopted thresholds before the pilot. Release 2 requires separate draft and recovery evidence. Release 3 requires complete coverage for the selected calendar interval.
