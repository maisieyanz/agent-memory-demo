---
description: "Runbook for triaging a production incident"
---

## Triage Steps
1. Check the alarm dashboard — identify the breaching metric
2. Filter logs by the request id from the alarm
3. Follow traces across service boundaries
4. Correlate onset with deployments from the last two hours

## Rules
- Never restart a service before understanding the root cause
- Capture a heap dump before restarting anything memory-related
- Document findings in the incident channel before acting
