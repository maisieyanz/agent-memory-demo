# Consolidation Changelog

## 2026-08-14 19:20

Operations: deduplicate, resolveContradictions, deriveInsights, reorganize
Actions (3):
  - merge: facts/dark-mode-preference.md + facts/theme-setting.md + facts/user-prefers-dark-mode-over-light-mode.md → facts/dark-theme-preference.md (Three files independently record the same dark-mode preference fact (one plain, one with a stated reason). Consolidated into a single, more complete file to eliminate redundancy.)
  - delete: facts/indentation-tabs.md (Contradicted by facts/indentation-spaces.md, which explicitly states the user switched from tabs to 2-space indentation in June 2026, superseding this March 2026 record.)
  - merge: facts/testing-integration-preference.md + facts/testing-mock-boundaries.md + facts/testing-real-database.md → facts/testing-strategy-avoid-mocking.md (The three separate testing-preference facts, taken together, reveal a single higher-level policy driven by specific past incidents. Synthesizing them into one insight file captures the 'why' behind the preferences and removes now-redundant standalone notes.)

Summary: Reviewed 10 knowledge files. Found three duplicate dark-mode-preference facts and merged them into one complete file (facts/dark-theme-preference.md). Found a direct contradiction between indentation-tabs.md and indentation-spaces.md; deleted the outdated tabs record since the spaces file is explicitly newer (June 2026) and states it supersedes tabs. Found three related testing-preference facts (integration over unit tests, mocking only at HTTP boundaries, real database over mocks) that together…(+308 chars)
