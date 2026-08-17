---
description: "Team testing philosophy: favor real integration tests, minimize mocking"
---

## Pattern
The team consistently favors testing against real behavior over relying on mocks, based on repeated incidents where mocked tests gave false confidence:

- API layers are tested with integration tests rather than unit tests.
- Mocking is restricted to HTTP boundaries only; module-level mocking is disallowed because mock divergence caused a Q1 incident.
- Database interactions are tested against a real local database, not mocks — mocked tests passed last quarter while the underlying production migration still failed.

## Guidance
When writing tests, prefer real dependencies (real DB, real internal modules) and reserve mocking for external HTTP boundaries only. This policy exists specifically to prevent mock/reality divergence from masking real failures.
