# Consolidation Changelog

## 2026-08-18 14:18

Operations: deduplicate, resolveContradictions, deriveInsights, reorganize
Actions (3):
  - merge: facts/dark-mode-preference.md + facts/theme-setting.md + facts/user-prefers-dark-mode-over-light-mode.md → facts/theme-setting.md (These three files all state the same underlying fact (preference for dark mode/theme) with varying detail. Merged into the most complete version, combining the scope (editors/terminals/dev tools) with the stated rationale (eye strain), eliminating redundancy.)
  - delete: facts/indentation-tabs.md (Contradicts the more recent indentation-spaces.md (June 2026), which explicitly states the user switched from tabs to spaces, superseding this March 2026 fact. The outdated tabs preference is removed to avoid conflicting guidance.)
  - merge: facts/testing-integration-preference.md + facts/testing-mock-boundaries.md + facts/testing-real-database.md → facts/testing-avoid-mocks-philosophy.md (The three separate testing facts (integration over unit tests, mock only at HTTP boundaries, use a real database) together reveal a single higher-level testing philosophy driven by past incidents. Synthesizing them into one insight file captures the pattern and its rationale, fully superseding the fragmented originals.)

Summary: Reviewed 10 knowledge files. Consolidated three redundant dark-mode/theme preference files into the most complete version (facts/theme-setting.md), keeping scope and rationale. Resolved a contradiction between two indentation preference files by deleting the outdated tabs-based fact (March 2026) since it was explicitly superseded by the spaces fact (June 2026). Synthesized three related testing-preference files (integration over unit tests, mock boundary rules, real database testing) into a sing…(+254 chars)
