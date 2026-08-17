---
description: "Team testing strategy: minimize mocking, favor real integration tests"
---

## Strategy
The team has shifted toward integration-style testing and away from heavy mocking, based on direct incident experience:

- Prefer integration tests over unit tests for API layers.
- Test database interactions against a real local database rather than mocking the database — mocked DB tests passed last quarter while the actual production migration failed.
- When mocking is unavoidable, mock only at HTTP boundaries, never at the module level — module-level mock divergence caused a Q1 incident.

## Rationale
Mocks that diverge from real behavior have twice caused production issues to be missed in testing. The team's policy is now to test against real dependencies wherever practical and limit mocking to well-defined external boundaries.
