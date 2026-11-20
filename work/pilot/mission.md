# Release 1 mission

**Design baseline:** [Mail and Calendar Assistant Service Design and Architecture, version 3](../../docs/design/service-v3.md), November 19, 2026.

**Outcome:** A private user can see what they owe and what they await. The service reads one Gmail account, produces two daily private web briefings, and preserves local corrections.

**Scope:** Include Sent mail in the declared interval. Show incomplete coverage first. Keep known due work available during provider outages. Store permitted structured facts and references. Generate source descriptions transiently.

**Deferred work:** Release 2 adds user-requested, reviewed provider drafts. Release 3 adds selected calendars. Sending, forwarding, mail deletion, mail rules, and calendar mutation are outside the service contract.

**Human decisions:** Name the operator and privacy owner. Record eligibility, scope, source window, paused-account expiry, processors, key service, deployment costs, and evaluation thresholds before enrollment.

**Approval:** Repository setup only. The design remains proposed. Record implementation approval against a ticket or plan revision. Record pilot enrollment and release decisions separately.

**Acceptance:** Use the [pilot evidence guide](../../docs/acceptance/README.md) and the gate table in the version 3 design.
