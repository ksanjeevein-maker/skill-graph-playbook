# Queue Health Versus Root Cause

Use this note when dashboards show stress but the real operational problem is still unclear.

Queue metrics are important, but they are not the whole system. Follow [[triage-severity]] to decide whether the situation is urgent enough to change handling right now, and read [[runbook-drift]] when recurring backlog spikes suggest the procedure itself no longer matches reality.

## Key Rule

Treat queue health as a signal to investigate, not as proof of the cause.

## Inputs

- backlog size
- age distribution
- repeat failure patterns

## Outputs

- whether to escalate
- whether to investigate process drift
- whether to change staffing or routing temporarily
