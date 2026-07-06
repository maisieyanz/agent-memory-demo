---
description: "Step-by-step production debugging runbook"
---

# Production Debugging

## Triage Steps
1. Check the alarm dashboard — identify which metric is breaching
2. CloudWatch Logs: filter by request-id from the alarm
3. X-Ray traces: follow the request through service boundaries
4. Check recent deployments (last 2h) — correlate with error onset

## Rules
- Never restart a service without understanding the root cause
- Always capture a heap dump before restarting if memory-related
- Page the on-call for the upstream service if the issue crosses boundaries
- Document findings in the incident channel before taking action

## Common Patterns
- Timeout spikes → check downstream service health
- OOM kills → check for memory leaks in recent deploys (heap dump)
- 5xx burst → check if a bad deploy went through (rollback first, investigate second)