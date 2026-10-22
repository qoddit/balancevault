# Testing and Release

- [[test_all.c]] contains the C test suite in the available snapshot.
- [[ci.yml]] defines the CI workflow.
- [[release.yml]] defines the GitHub release workflow.
- [[release.sh]] contains release scripting.
- [[VERIFY_SOURCE.sh]] is a source verification script.
- [[CHANGELOG.md]] records release notes.
- [[VERSION]] and [[version.h]] carry version information.

## Release hygiene
Build artifacts should generally be published as GitHub Release assets rather than committed into the source tree. Confirm `git status`, version metadata, checksums, and a clean build before tagging. See [[VERSIONING.md]] and [[Known Issues and Verification]].
