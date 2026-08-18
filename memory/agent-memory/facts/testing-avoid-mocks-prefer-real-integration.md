---
description: "Team avoids mocking in favor of real integration tests, after mock-related production incidents"
---

The team has moved away from unit-test mocking toward real integration testing, driven by past incidents where mocks diverged from reality:

- API layers are tested with integration tests rather than unit tests.
- Mocking is restricted to HTTP boundaries only; module-level mocking is disallowed because mock divergence caused a Q1 incident.
- Database interactions are tested against a real local database instead of mocks, since mocked tests passed last quarter while the production migration still failed.

**Pattern:** mocks that diverge from real behavior have repeatedly caused production issues, so the team's testing strategy now favors exercising real dependencies (real DB, real HTTP-boundary-only mocking, integration over unit tests for APIs) whenever feasible.
