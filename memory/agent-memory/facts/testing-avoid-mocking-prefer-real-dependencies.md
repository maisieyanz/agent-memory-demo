---
description: "Team avoids mocking and favors real dependencies in tests, based on past incidents"
---

## Insight
The team has moved toward testing against real dependencies rather than mocks, driven by concrete incidents where mocked tests passed but production failed.

## Supporting Facts
- Integration tests are preferred over unit tests for API layers.
- Mocking is only acceptable at HTTP boundaries, never at the module level — mock divergence at the module level caused a Q1 incident.
- Database interactions should be tested against a real local database, not mocks — mocked tests passed last quarter while the production migration still failed.

## Takeaway
When writing tests, prefer real integration paths (real DB, real service calls) and limit mocking to external HTTP boundaries only.
