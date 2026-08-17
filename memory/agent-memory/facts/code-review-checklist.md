---
description: "Code review checklist: what to always flag"
---

## Always Flag
- Unvalidated user input reaching a database query
- Secrets or API keys committed to source
- Missing error handling on async operations
- Breaking public API changes without a version bump
- Tests that mock the very thing they claim to verify

## Common Nits
- Inconsistent naming, dead code, leftover debug logging
- Magic numbers without named constants
