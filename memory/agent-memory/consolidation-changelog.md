# Consolidation Changelog

## 2026-08-18 06:19

Operations: deduplicate, resolveContradictions, deriveInsights, reorganize
Actions (3):
  - merge: facts/dark-mode-preference.md + facts/theme-setting.md + facts/user-prefers-dark-mode-over-light-mode.md → facts/dark-mode-preference.md (Three files all state the same underlying fact (dark mode preference); theme-setting.md adds the reason (eye strain) and dark-mode-preference.md adds scope (editors/terminals/dev tools). Merged into one complete file, redundant sources removed.)
  - delete: facts/indentation-tabs.md (Contradicted by indentation-spaces.md, which is more recent (June 2026) and explicitly states it supersedes the tabs preference recorded in March 2026.)
  - merge: facts/testing-integration-preference.md + facts/testing-mock-boundaries.md + facts/testing-real-database.md → facts/testing-philosophy.md (The three testing facts individually describe isolated preferences, but together they reveal a single higher-level policy (avoid mocks, test against real systems) driven by two documented incidents. Synthesizing them into one insight file captures this pattern more usefully than three fragmented facts.)

Summary: Consolidated three duplicate dark-mode preference files into one complete fact, removed the outdated tabs-indentation file superseded by the newer spaces preference, and synthesized three related testing facts (integration tests, real database, mock boundaries) into a single 'testing philosophy' insight file explaining the team's mock-avoidance policy. Left the code review checklist and production runbook untouched as they are unique, well-formed, and non-redundant.
