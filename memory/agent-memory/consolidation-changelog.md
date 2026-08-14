# Consolidation Changelog

## 2026-08-14 18:52

Operations: deduplicate, resolveContradictions, deriveInsights, reorganize
Actions (3):
  - merge: facts/dark-mode-preference.md + facts/theme-setting.md + facts/user-prefers-dark-mode-over-light-mode.md → facts/theme-setting.md (Three files all express the same underlying fact (user prefers dark mode/theme). Merged into the most complete version, which also retains the rationale (eye strain) that the other two lacked.)
  - delete: facts/indentation-tabs.md (Contradicts indentation-spaces.md. The spaces file is more recent (June 2026) and explicitly states it supersedes the tabs preference recorded in March 2026, so the outdated tabs fact is removed.)
  - merge: facts/testing-integration-preference.md + facts/testing-mock-boundaries.md + facts/testing-real-database.md → facts/testing-avoid-mocking-prefer-real-dependencies.md (These three testing facts individually describe isolated rules, but together they reveal a higher-level pattern: the team deliberately avoids mocking in favor of realistic tests because mocking previously caused production incidents. Synthesizing them into one insight file captures this pattern while preserving all supporting specifics, fully superseding the three source files.)

Summary: Consolidated three duplicate dark-mode/theme preference files into the most complete one (facts/theme-setting.md). Removed the outdated tabs-indentation fact since the spaces-indentation fact (June 2026) explicitly supersedes it. Synthesized three related testing facts (integration over unit tests, mock only at HTTP boundaries, test against real DB) into a single derived insight file explaining the team's overall anti-mocking testing philosophy, superseding the individual fact files. Left the co…(+94 chars)
