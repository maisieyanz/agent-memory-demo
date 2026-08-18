---
description: "Team prefers testing against real dependencies over mocks, especially for API and database layers"
---

## Pattern
The team has a strong preference for testing against real systems rather than mocks, learned from past incidents:

- Integration tests are preferred over unit tests for API layers.
- Database interactions are tested against a real local database, not mocks — mocked tests passed last quarter while the production migration still failed.
- Mocking is acceptable only at HTTP boundaries, never at the module level — mock divergence at the module level caused a Q1 incident.

## Takeaway
Avoid mocking internal components (databases, modules); reserve mocking for external HTTP boundaries only. This reduces the risk of tests passing while production behavior diverges.
