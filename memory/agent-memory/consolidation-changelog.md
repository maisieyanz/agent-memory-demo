# Consolidation Changelog

## 2026-08-17 06:31

Operations: deduplicate, resolveContradictions, deriveInsights, reorganize
Actions (4):
  - merge: facts/dark-mode-preference.md + facts/theme-setting.md + facts/user-prefers-dark-mode-over-light-mode.md → facts/dark-mode-preference.md (Three files independently stated the same dark-mode preference fact with varying detail. Merged into one complete file that keeps the scope (all tools) and the rationale (eye strain), eliminating redundancy.)
  - update: facts/indentation-spaces.md (indentation-tabs.md (March 2026) and indentation-spaces.md (June 2026) directly contradict each other. The spaces preference is more recent and explicitly states it supersedes tabs, so it is kept and clarified; the outdated tabs file is removed.)
  - delete: facts/indentation-tabs.md (Superseded by the more recent June 2026 switch to 2-space indentation documented in indentation-spaces.md; keeping both creates a direct contradiction.)
  - merge: facts/testing-integration-preference.md + facts/testing-mock-boundaries.md + facts/testing-real-database.md → facts/testing-avoid-mocks-strategy.md (The three separate testing facts (integration over unit tests, mocking only at HTTP boundaries, testing against a real database) together reveal a single higher-level testing philosophy driven by past incidents. Synthesized into one insight file rather than three fragmented facts.)

Summary: Consolidated redundant dark-mode preference facts into one complete file, resolved the tabs-vs-spaces indentation contradiction by keeping the more recent 2-space policy and deleting the outdated tabs file, and synthesized three related testing facts (integration over unit tests, HTTP-only mocking, real database testing) into a single derived insight file describing the team's incident-driven anti-mocking testing strategy. Left the code review checklist and production debugging runbook untouched…(+52 chars)
