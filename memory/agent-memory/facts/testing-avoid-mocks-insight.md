---
description: "Team avoids mocking internals; prefers real integration tests due to past incidents"
---

The team has moved away from mock-heavy unit testing for API layers in favor of integration tests that exercise real dependencies:

- API layers are tested with integration tests rather than unit tests.
- Database interactions are tested against a real local database, not mocks — a mocked test suite passed last quarter while the production migration it should have caught actually failed.
- Mocking is restricted to HTTP boundaries only; module-level mocking is disallowed because mock divergence from real behavior caused a Q1 incident.

Insight: repeated incidents where mocks diverged from real system behavior led the team to adopt a policy of testing against real components wherever feasible, limiting mocks strictly to external HTTP boundaries.
