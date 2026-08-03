# Consolidation Changelog

## 2026-08-03 14:30

Operations: deduplicate, resolveContradictions, deriveInsights, reorganize
Actions (3):
  - merge: facts/dark-mode-preference.md + facts/theme-setting.md → facts/theme-dark-mode.md (Both files express the same core fact (dark mode preference) from complementary angles (scope of application vs. underlying reason). Merged into a single comprehensive fact file to eliminate redundancy while preserving all details.)
  - delete: facts/indentation-tabs.md (Contradicted by facts/indentation-spaces.md, which explicitly states the user switched from tabs to 2-space indentation in June 2026, superseding the March 2026 tabs preference. The outdated fact is removed.)
  - merge: facts/testing-integration-preference.md + facts/testing-mock-boundaries.md + facts/testing-real-database.md → facts/testing-avoid-mocks-philosophy.md (These three facts individually describe isolated testing preferences, but together they reveal a higher-level team philosophy of minimizing mocking and preferring real dependencies, motivated by concrete past incidents. Synthesized into a single insight file that fully captures and supersedes the individual facts.)

Summary: Consolidated the 10 knowledge files by merging duplicate dark-mode/theme preferences into a single fact, deleting the outdated tabs-indentation fact that was contradicted by a more recent spaces-indentation update, and synthesizing three related testing-preference facts (integration over unit tests, HTTP-only mocking, real database testing) into one higher-level 'avoid mocks' philosophy file. Skill and persona files (code-review, debugging-production, persona) were left unchanged as they serve d…(+32 chars)
