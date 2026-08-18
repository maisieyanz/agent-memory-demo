# Consolidation Changelog

## 2026-08-18 05:30

Operations: deduplicate, resolveContradictions, deriveInsights, reorganize
Actions (3):
  - merge: facts/dark-mode-preference.md + facts/theme-setting.md + facts/user-prefers-dark-mode-over-light-mode-for-uitheme.md → facts/dark-mode-preference.md (All three files state the same underlying fact (preference for dark mode/theme). Merged into one file that keeps the scope (editors/terminals/dev tools) from dark-mode-preference.md and the rationale (eye strain) from theme-setting.md, eliminating redundant near-duplicate facts.)
  - delete: facts/indentation-tabs.md (Contradicted by indentation-spaces.md, which records a more recent (June 2026) update explicitly superseding the tabs preference from March 2026. The outdated fact is removed to avoid conflicting guidance.)
  - merge: facts/testing-integration-preference.md + facts/testing-mock-boundaries.md + facts/testing-real-database.md → facts/testing-avoid-mocks-prefer-real-integration.md (These three facts individually describe isolated testing preferences, but together they reveal a higher-level, incident-driven pattern: the team systematically avoids mocking wherever it previously caused failures. Synthesizing them into one insight file captures this pattern without losing any of the specific supporting details.)

Summary: Consolidated three near-duplicate dark-mode/theme preference files into a single richer fact. Deleted the outdated tabs-indentation fact that is contradicted by the more recent spaces-indentation update. Synthesized three related testing-preference facts (integration over unit tests, HTTP-only mocking, real database testing) into one derived insight file describing the team's incident-driven avoidance of mocking. Left the code-review-checklist and production-runbook files unchanged as they are d…(+40 chars)
