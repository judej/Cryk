# Diagnosis

State the observed symptom, affected entry point, data scope, and revision. Use synthetic data or approved content-free measurements.

1. Establish a repeatable baseline. Record input size, concurrency, elapsed time, and measurement limits.
2. Separate provider lag, queue wait, analysis time, and user-visible delay. Identify the largest measured contribution.
3. Compare equivalent runs. For a due-work delay, include the result while synchronization or analysis is busy.
4. Propose the smallest change supported by evidence. Define a target and a repeat measurement with the same workload.
5. Include checks for lost work, duplicate results, tenant isolation, and preservation of user corrections where applicable.

Return findings and a plan. A request for diagnosis authorizes investigation. Ask for implementation approval when needed.
