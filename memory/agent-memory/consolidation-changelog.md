# Consolidation Changelog

## 2026-08-03 14:28

Operations: deduplicate, resolveContradictions, deriveInsights, reorganize
Actions (3):
  - delete: facts/indentation-tabs.md (Contradicts the more recent indentation-spaces.md (June 2026 update supersedes the March 2026 tabs preference, which was explicitly replaced along with .editorconfig and Prettier config).)
  - merge: facts/dark-mode-preference.md + facts/theme-setting.md → facts/dark-mode-theme-preference.md (Both files express the same underlying fact (preference for dark mode/theme); merged to keep the scope detail (editors/terminals/dev tools) together with the rationale (eye strain) in one complete record, eliminating redundancy.)
  - merge: facts/testing-integration-preference.md + facts/testing-mock-boundaries.md + facts/testing-real-database.md → facts/testing-avoid-mocks-prefer-real-dependencies.md (The three individual testing facts (integration over unit tests, HTTP-only mocking, real database testing) together reveal a single higher-level testing philosophy driven by past incidents; synthesizing them into one insight file fully captures and supersedes the individual notes.)

Summary: Reviewed 10 knowledge files. Found one direct contradiction (indentation: tabs vs. spaces) resolved by deleting the outdated tabs preference in favor of the more recent spaces preference. Found one duplicate fact (dark mode/theme preference) merged into a single complete file retaining both scope and rationale. Found three related testing facts (integration tests over unit tests, HTTP-only mocking, real database testing) that together reveal a higher-level team testing philosophy of minimizing m…(+284 chars)
