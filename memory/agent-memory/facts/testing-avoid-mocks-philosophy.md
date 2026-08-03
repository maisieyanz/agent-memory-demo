---
description: "Team philosophy: avoid mocks, test against real dependencies/boundaries"
---

Across the API layer and database interactions, the team has converged on a consistent testing philosophy: prefer exercising real dependencies over mocking internals.

- Integration tests are preferred over unit tests for API layers.
- Mocking is only acceptable at HTTP boundaries, never at the module level. Mock divergence from real behavior at the module level caused a Q1 incident.
- Database interactions should be tested against a real local database rather than mocks. Mocked tests passed last quarter while the production migration actually failed, revealing the risk of over-mocking.

Overall pattern: mocks are only trusted at true external I/O boundaries; everything else should be tested against real, representative behavior to avoid false confidence.
