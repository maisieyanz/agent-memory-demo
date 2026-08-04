# Consolidation Changelog

## 2026-08-03 15:32

Operations: deduplicate, resolveContradictions, deriveInsights, reorganize
Actions (3):
  - merge: facts/dark-mode-preference.md + facts/theme-setting.md → facts/theme-setting.md (Both files state the same core preference for dark mode/theme; merged into one file that keeps the broader scope (editors, terminals, dev tools) and the underlying reason (eye strain), eliminating redundancy.)
  - delete: facts/indentation-tabs.md (Contradicted by facts/indentation-spaces.md, which is more recent (June 2026) and explicitly states the user switched from tabs to spaces, superseding this outdated March 2026 fact.)
  - merge: facts/testing-integration-preference.md + facts/testing-mock-boundaries.md + facts/testing-real-database.md → facts/testing-avoid-mocks-strategy.md (These three facts individually describe isolated testing preferences, but together they reveal a higher-level pattern: the team systematically avoids mocking beyond HTTP boundaries because it has caused real incidents. Synthesizing them into one insight file preserves all original details (Q1 incident, migration failure) while capturing the overarching rationale.)

Summary: Reviewed 9 knowledge files. Merged two duplicate dark-mode/theme preference files into the more detailed theme-setting.md. Deleted the outdated tabs-indentation fact, which was explicitly superseded by the more recent spaces-indentation fact. Synthesized three separate testing-preference facts (integration over unit tests, HTTP-only mocking, real database testing) into a single derived insight file capturing the team's overarching anti-mocking testing philosophy, while preserving all underlying …(+143 chars)

## 2026-08-04 15:59

Operations: deduplicate, resolveContradictions, deriveInsights, reorganize
Actions (3):
  - delete: facts/indentation-tabs.md (Contradicted by facts/indentation-spaces.md, which records that the user switched from tabs to 2-space indentation in June 2026 (more recent, and explicitly states it supersedes tabs). The March 2026 tabs preference is now outdated.)
  - merge: facts/dark-mode-preference.md + facts/theme-setting.md → facts/dark-theme-preference.md (Both files express the same underlying fact (preference for dark theme/mode). theme-setting.md adds the causal reason (eye strain) missing from dark-mode-preference.md, so they are merged into one complete fact file and the redundant originals removed.)
  - merge: facts/testing-avoid-mocks-strategy.md + facts/testing-integration-preference.md + facts/testing-mock-boundaries.md + facts/testing-real-database.md → facts/testing-strategy.md (testing-avoid-mocks-strategy.md already synthesizes and fully restates the facts in testing-integration-preference.md, testing-mock-boundaries.md, and testing-real-database.md as a higher-level insight. The three narrower files are fully superseded by this synthesis, so they are consolidated into one authoritative strategy file and the redundant sources removed.)

Summary: Reviewed 10 knowledge files. Deleted the outdated tabs-indentation fact, which is contradicted by a more recent (June 2026) switch to spaces already documented elsewhere. Merged two overlapping dark-theme preference files into one complete fact that keeps the added rationale (eye strain). Consolidated four testing-related files into a single testing-strategy file, since one file already synthesized the other three as a higher-level insight, making the narrower files redundant. Left the code-revi…(+109 chars)
