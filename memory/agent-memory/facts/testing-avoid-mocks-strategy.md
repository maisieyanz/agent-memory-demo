---
description: "Team's overall testing philosophy: avoid mocks, test against real dependencies"
---

## Pattern
The team has converged on testing against real dependencies rather than mocks, after mocking caused multiple production incidents.

## Specifics
- Integration tests are preferred over unit tests for API layers.
- Mocking is acceptable only at HTTP boundaries, never at the module level — mock divergence at the module level caused a Q1 incident.
- Database interactions are tested against a real local database rather than mocks — mocked tests passed last quarter while the production migration still failed.

## Insight
Mocking below the HTTP boundary (e.g., module-level or database mocks) has repeatedly hidden real failures. The team's policy of favoring integration tests and real local dependencies is a direct response to these incidents.
