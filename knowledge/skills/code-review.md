---
description: "Code review checklist and patterns to flag"
---

# Code Review Patterns

## Always Flag
- Unvalidated user input reaching a database query
- Secrets or API keys in source code
- Missing error handling on async operations
- Breaking changes to public API without version bump
- Tests that mock the thing they claim to test

## Common Nits
- Inconsistent naming (camelCase vs snake_case mix)
- Dead code or commented-out blocks
- Console.log left in production code
- Magic numbers without named constants

## Positive Patterns to Acknowledge
- Good separation of concerns
- Defensive error handling
- Clear, descriptive variable names
- Tests that cover edge cases, not just happy path