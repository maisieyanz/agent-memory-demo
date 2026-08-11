# Consolidation Changelog

## 2026-08-11 14:51

Operations: deduplicate, resolveContradictions, deriveInsights, reorganize
Actions (3):
  - merge: facts/dark-mode-preference.md + facts/theme-setting.md → facts/theme-preference.md (Both files describe the same dark-theme preference; theme-setting.md adds the underlying rationale (eye strain), so they are merged into a single complete fact and the redundant file removed.)
  - delete: facts/indentation-tabs.md (Contradicted and superseded by facts/indentation-spaces.md, which explicitly states the user switched from tabs to 2-space indentation in June 2026 (later than the March 2026 tabs record).)
  - merge: facts/testing-integration-preference.md + facts/testing-mock-boundaries.md + facts/testing-real-database.md → facts/testing-philosophy.md (The three testing files individually describe integration-over-unit preference, real-database testing, and HTTP-only mocking boundaries. Together they reveal a single higher-level testing philosophy driven by two real incidents, so they are synthesized into one insight file that supersedes the separate facts.)

Summary: Merged the two dark-theme preference files (dark-mode-preference.md and theme-setting.md) into a single theme-preference.md that keeps both the preference and its rationale. Deleted the outdated indentation-tabs.md fact since it is contradicted by the more recent (June 2026) indentation-spaces.md switch to spaces. Synthesized the three separate testing-related facts (integration preference, mock boundaries, real database) into one higher-level testing-philosophy.md that captures the team's overa…(+266 chars)
