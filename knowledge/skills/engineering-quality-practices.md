---
description: "Derived insight: cross-cutting engineering quality and safety principles spanning code review and production operations"
---

# Engineering Quality Practices — Derived Insights

> This file captures higher-level patterns derived from `code-review.md` and `debugging-production.md`.

## Core Theme: Catch Problems Early, Respond Deliberately

Both code review and production debugging share a common discipline:
- **Shift left on risk** — flag security, error-handling, and API contract issues at review time before they reach production.
- **Never act blindly under pressure** — in production, understand root cause before restarting services, just as in reviews you flag bad patterns rather than silently ignoring them.

## Layered Defence Pattern

| Layer | Practice | Source |
|---|---|---|
| Code Review | Flag unvalidated input, missing error handling, secrets in code | `code-review.md` |
| Code Review | Acknowledge good separation of concerns and defensive patterns | `code-review.md` |
| Production | Correlate errors with recent deploys before acting | `debugging-production.md` |
| Production | Capture heap dumps before restarts; document before acting | `debugging-production.md` |

## Shared Anti-Patterns to Avoid
- Skipping error handling (flagged in review *and* a root cause of OOM/5xx in prod)
- Acting without understanding (restarting without root cause = same failure as merging without review)
- Ignoring boundaries (API version bumps in review ↔ paging upstream on-call in prod)

## Key Heuristics
1. **Security first**: Unvalidated input and hardcoded secrets are always blockers, never nits.
2. **Correlate before concluding**: In production, check recent deploys; in reviews, check the full call chain.
3. **Document the finding**: Incident channel entries in prod mirror review comments — the reasoning matters as much as the fix.
4. **Tests must be honest**: Mocks that test themselves are as dangerous as a monitoring alert with no runbook.
