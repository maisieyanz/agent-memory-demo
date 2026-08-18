---
description: "Team testing philosophy: minimize mocking, favor real dependencies"
---

## Pattern
The team has converged on a philosophy of testing against real dependencies rather than mocks, driven by concrete incidents where mocked tests diverged from production behavior:

- Integration tests are preferred over unit tests for API layers.
- Mocking is only acceptable at HTTP boundaries — never at the module level. Mock divergence at the module level caused a Q1 incident.
- Database interactions should be tested against a real local database, not mocks. Mocked tests passed last quarter while the corresponding production migration still failed.

## Takeaway
Mocks are treated as a source of false confidence for this team; prefer real integration points (real DB, real service calls except at the outer HTTP boundary) whenever feasible.
