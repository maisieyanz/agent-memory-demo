---
description: "Team testing philosophy: minimize mocking, test against real dependencies"
---

The team has converged on a broader testing philosophy after being burned by mock-based false confidence:

- Prefer integration tests over unit tests for API layers.
- Mock only at HTTP boundaries, never at the module level — mock divergence at the module level caused a Q1 incident.
- Test database interactions against a real local database rather than mocks — mocked tests passed last quarter while the production migration still failed.

Overall pattern: minimize mocking and validate behavior against real dependencies (real databases, real API integration paths) wherever practical, reserving mocks strictly for external HTTP boundaries.
