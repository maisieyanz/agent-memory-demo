---
description: "Team prefers realistic testing over mocking, based on past incidents"
---

## Pattern
The team consistently avoids relying on mocks in favor of testing against real dependencies:
- Integration tests are preferred over unit tests for API layers.
- Mocking is acceptable only at HTTP boundaries, never at the module level.
- Database interactions are tested against a real local database rather than mocked.

## Why
This pattern emerged from repeated incidents where mocked tests passed but production failed:
- Mock divergence at the module level caused a Q1 incident.
- Mocked database tests passed last quarter while the production migration still failed.

The overarching lesson: prefer realistic test setups (real DB, integration tests, HTTP-boundary-only mocking) because mocks that diverge from real behavior have repeatedly hidden production-breaking bugs.
