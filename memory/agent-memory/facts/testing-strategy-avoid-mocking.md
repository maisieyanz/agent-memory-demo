---
description: "Team avoids mocking in favor of realistic tests, based on past incidents"
---

The team's testing strategy has converged on minimizing mocking after repeated incidents where mocked tests passed but real behavior failed:

- Prefer integration tests over unit tests for API layers.
- Mocking is acceptable only at HTTP boundaries, never at the module level — mock divergence at the module level caused a Q1 incident.
- Test database interactions against a real local database rather than mocks — mocked tests passed last quarter while the production migration still failed.

**Insight:** For this team, mocks tend to hide real integration failures (database migrations, module-level divergence). The underlying policy is to test against real dependencies wherever practical, and reserve mocking strictly for external HTTP boundaries.
