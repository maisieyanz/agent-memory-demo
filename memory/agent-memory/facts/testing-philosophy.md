---
description: "Team testing philosophy: prefer real dependencies and integration tests over heavy mocking, due to past incidents caused by mock divergence"
---

## Guiding Principle
The team favors testing against real dependencies and real behavior rather than extensive mocking, because mock divergence from reality has previously caused production incidents.

## Specific Practices
- Integration tests are preferred over unit tests for API layers.
- Mocking is acceptable only at HTTP boundaries, never at the module level — module-level mock divergence caused a Q1 incident.
- Database interactions are tested against a real local database, not mocks — mocked tests passed last quarter while the production migration still failed.

## Rationale
These three practices are all instances of the same underlying policy: minimize reliance on mocks that can silently diverge from real system behavior, and validate against real infrastructure wherever practical.
