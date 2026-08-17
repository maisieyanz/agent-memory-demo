# Consolidation Changelog

## 2026-08-17 19:38

Operations: deduplicate, resolveContradictions, deriveInsights, reorganize
Actions (3):
  - merge: facts/dark-mode-preference.md + facts/theme-setting.md + facts/user-prefers-dark-mode-over-light-mode.md → facts/dark-mode-preference.md (All three files state the same underlying fact (preference for dark mode); theme-setting.md additionally supplies the rationale (eye strain). Merged into a single complete fact file to eliminate redundancy.)
  - delete: facts/indentation-tabs.md (Contradicted and superseded by indentation-spaces.md, which records a later (June 2026) change away from tabs to 2-space indentation. Outdated fact removed in favor of the more recent one.)
  - merge: facts/testing-integration-preference.md + facts/testing-mock-boundaries.md + facts/testing-real-database.md → facts/testing-philosophy.md (The three testing facts individually describe isolated preferences, but together they reveal a single higher-level policy: the team deliberately minimizes mocking in favor of real integration testing due to past incidents. Synthesizing them into one insight file captures this pattern without losing the supporting details, which are preserved in the merged content.)

Summary: Reviewed 10 knowledge files. Found three files expressing the same dark-mode preference fact (with theme-setting.md adding the eye-strain rationale) and merged them into a single consolidated fact. Found a direct contradiction between indentation-tabs.md (March 2026) and indentation-spaces.md (June 2026); deleted the outdated tabs record since spaces supersedes it. Identified that the three testing-related files (integration-over-unit, mock-boundaries, real-database) together reveal a single und…(+341 chars)
