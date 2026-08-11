---
description: "Team testing philosophy: avoid mocking, test against real systems"
---

## Guiding Principle
The team favors integration-style tests that exercise real systems over unit tests that rely on mocks, especially for API layers and database interactions.

## Rules
- Prefer integration tests over unit tests for API layers.
- Test database interactions against a real local database rather than mocking the database.
- Mocking is acceptable only at HTTP boundaries; never mock at the module level internally.

## Why
- Mocked database tests passed last quarter while the production migration still failed, exposing the risk of over-mocking.
- Mock divergence at the module level caused a separate Q1 incident.

Together these incidents established the current policy: rely on real dependencies wherever feasible, and restrict mocking to external HTTP boundaries only.
