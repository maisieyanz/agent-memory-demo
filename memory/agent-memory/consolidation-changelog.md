# Consolidation Changelog

## 2026-08-03 15:32

Operations: deduplicate, resolveContradictions, deriveInsights, reorganize
Actions (3):
  - merge: facts/dark-mode-preference.md + facts/theme-setting.md → facts/theme-setting.md (Both files state the same core preference for dark mode/theme; merged into one file that keeps the broader scope (editors, terminals, dev tools) and the underlying reason (eye strain), eliminating redundancy.)
  - delete: facts/indentation-tabs.md (Contradicted by facts/indentation-spaces.md, which is more recent (June 2026) and explicitly states the user switched from tabs to spaces, superseding this outdated March 2026 fact.)
  - merge: facts/testing-integration-preference.md + facts/testing-mock-boundaries.md + facts/testing-real-database.md → facts/testing-avoid-mocks-strategy.md (These three facts individually describe isolated testing preferences, but together they reveal a higher-level pattern: the team systematically avoids mocking beyond HTTP boundaries because it has caused real incidents. Synthesizing them into one insight file preserves all original details (Q1 incident, migration failure) while capturing the overarching rationale.)

Summary: Reviewed 9 knowledge files. Merged two duplicate dark-mode/theme preference files into the more detailed theme-setting.md. Deleted the outdated tabs-indentation fact, which was explicitly superseded by the more recent spaces-indentation fact. Synthesized three separate testing-preference facts (integration over unit tests, HTTP-only mocking, real database testing) into a single derived insight file capturing the team's overarching anti-mocking testing philosophy, while preserving all underlying …(+143 chars)
