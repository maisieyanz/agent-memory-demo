---
description: "Team testing philosophy: integration-first, real dependencies, mock only at HTTP boundaries"
---

## General Approach
The team favors integration tests over unit tests for API layers.

## Database Testing
Test database interactions against a real (local) database, not mocks. Mocked DB tests passed last quarter but the prod migration still failed — real databases catch what mocks miss.

## Mocking Policy
Mock only at HTTP/system boundaries; never at the module level. Mock divergence caused issues in Q1, reinforcing this rule.
