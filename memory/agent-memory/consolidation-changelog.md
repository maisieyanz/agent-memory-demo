# Consolidation Changelog

## 2026-08-18 14:35

Operations: deduplicate, resolveContradictions, deriveInsights, reorganize
Actions (3):
  - merge: facts/dark-mode-preference.md + facts/theme-setting.md + facts/user-prefers-dark-mode-over-light-mode.md → facts/dark-mode-preference.md (These three files all state the same underlying fact (dark mode preference), with theme-setting.md adding the rationale (eye strain). Merged into a single complete file to eliminate redundancy.)
  - delete: facts/indentation-tabs.md (Contradicted by indentation-spaces.md, which explicitly states the user switched from tabs to 2-space indentation in June 2026 (more recent, supersedes tabs recorded March 2026).)
  - merge: facts/testing-integration-preference.md + facts/testing-mock-boundaries.md + facts/testing-real-database.md → facts/testing-prefers-real-dependencies.md (These three testing facts individually describe isolated preferences, but together they reveal a higher-level pattern: the team avoids mocking internal dependencies and prefers real integration testing due to prior incidents. Synthesizing them into one insight file captures this pattern more usefully than three separate facts.)

Summary: Consolidated redundant dark-mode preference facts into one complete file with rationale. Resolved the indentation contradiction by deleting the outdated tabs preference in favor of the more recent (June 2026) spaces preference. Synthesized three related testing-preference facts (integration tests, real database, HTTP-only mocking) into a single higher-level insight file describing the team's preference for testing against real dependencies over mocks. Left the code-review-checklist and debugging…(+96 chars)
