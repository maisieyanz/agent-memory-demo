# Consolidation Changelog

## 2026-08-17 22:06

Operations: deduplicate, resolveContradictions, deriveInsights, reorganize
Actions (3):
  - merge: facts/dark-mode-preference.md + facts/theme-setting.md + facts/user-prefers-dark-mode-over-light-mode.md → facts/dark-mode-preference.md (Three files all state the same core fact (dark mode preference) with overlapping/redundant wording. Merged into one file that keeps the broadest scope (editors/terminals/dev tools) and the underlying reason (eye strain), eliminating duplication.)
  - delete: facts/indentation-tabs.md (Contradicted by indentation-spaces.md, which records a more recent (June 2026) update where the user switched from tabs to 2-space indentation, explicitly superseding the March 2026 tabs preference.)
  - merge: facts/testing-integration-preference.md + facts/testing-mock-boundaries.md + facts/testing-real-database.md → facts/testing-avoid-mocks-insight.md (The three testing facts individually describe isolated preferences, but together they reveal a higher-level pattern: the team's testing strategy is driven by real incidents caused by mock divergence, leading to a deliberate policy of minimizing mocking. Synthesizing them into one insight file captures this pattern and fully supersedes the narrower originals.)

Summary: Reviewed 10 knowledge files. Consolidated three redundant dark-mode preference files into a single, more complete fact file. Resolved a contradiction between tabs vs. spaces indentation preferences by deleting the outdated (March 2026) tabs file in favor of the more recent (June 2026) spaces file. Synthesized three related testing-preference facts (integration over unit tests, real database over mocks, mocks restricted to HTTP boundaries) into a single derived insight file explaining the team's …(+186 chars)
