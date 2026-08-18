# Consolidation Changelog

## 2026-08-18 16:52

Operations: deduplicate, resolveContradictions, deriveInsights, reorganize
Actions (3):
  - merge: facts/dark-mode-preference.md + facts/prefers-dark-mode-over-light-mode.md + facts/theme-setting.md → facts/theme-dark-mode-preference.md (Three files (dark-mode-preference.md, prefers-dark-mode-over-light-mode.md, theme-setting.md) all state the same underlying fact - a preference for dark mode/theme. theme-setting.md adds the eye-strain rationale, so the merged file keeps all details (scope: editors/terminals/dev tools, plus the reason) while eliminating redundant near-duplicate files.)
  - delete: facts/indentation-tabs.md (Contradicts indentation-spaces.md. The spaces file is explicitly dated June 2026 and states it supersedes the tabs preference recorded in March 2026, so the outdated tabs fact should be removed in favor of the more recent, more specific record.)
  - merge: facts/testing-integration-preference.md + facts/testing-mock-boundaries.md + facts/testing-real-database.md → facts/testing-avoids-mocking-preference.md (The three testing files individually describe specific practices (integration over unit tests, mock only at HTTP boundary, real DB over mocks) that together reveal a higher-level pattern: the team's testing philosophy is driven by repeated incidents caused by mock divergence. Synthesizing them into one insight file captures this pattern while preserving the specific incident details, fully superseding the three narrower facts.)

Summary: Reviewed 10 knowledge files. Found three near-duplicate dark-mode/theme preference files and merged them into one complete file preserving both scope and rationale. Found a direct contradiction between an indentation-tabs fact (March 2026) and an indentation-spaces fact (June 2026, explicitly stated to supersede tabs) and deleted the outdated tabs file. Found three testing-related files (integration tests preference, mock-boundary rule, real-database preference) that together reveal a higher-lev…(+258 chars)
