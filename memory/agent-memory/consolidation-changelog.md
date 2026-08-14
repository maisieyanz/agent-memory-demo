# Consolidation Changelog

## 2026-08-14 18:12

Operations: deduplicate, resolveContradictions, deriveInsights, reorganize
Actions (3):
  - merge: facts/dark-mode-preference.md + facts/theme-setting.md → facts/theme-preference.md (Both files state the same dark-mode/theme preference; theme-setting.md adds the underlying reason (eye strain), so they are merged into one complete fact and the redundant originals removed.)
  - delete: facts/indentation-tabs.md (Contradicts the more recent indentation-spaces.md fact (June 2026), which explicitly states the user switched from tabs to spaces and supersedes this March 2026 record. Outdated fact removed to resolve the contradiction.)
  - merge: facts/testing-integration-preference.md + facts/testing-mock-boundaries.md + facts/testing-real-database.md → facts/testing-philosophy.md (The three testing files each describe a specific practice (integration over unit tests, HTTP-only mocking, real database testing) that are all facets of one overarching philosophy: avoid mocks that diverge from reality. Synthesizing them into a single insight file preserves all specific incident details while capturing the higher-level pattern, fully superseding the fragmented originals.)

Summary: Reviewed 9 knowledge files. Found two pairs of duplicate facts (dark mode preference / theme setting, and three testing-related facts) and one contradiction (tabs vs spaces indentation). Merged the dark-mode and theme-setting facts into a single richer preference file. Deleted the outdated tabs indentation fact since the spaces fact explicitly supersedes it as of June 2026. Synthesized the three testing facts (integration tests preference, HTTP-only mocking, real database testing) into a single …(+266 chars)
