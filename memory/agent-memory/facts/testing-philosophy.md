---
description: "Team testing philosophy: favor real integration tests over mocks"
---

## Principles
- Prefer integration tests over unit tests for API layers
- Test database interactions against a real local database, not mocks
- Mock only at HTTP boundaries, never at the module level

## Why This Matters
- Mocked tests passed last quarter while the production migration still failed
- Mock divergence at the module level caused a Q1 incident

Together these experiences show the team's core testing rule: minimize mocking and validate against real dependencies wherever practical, since mocks previously masked real failures.
