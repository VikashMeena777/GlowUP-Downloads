# GlowUP-Downloads

Public, download-only release repository for the Glow Up Android app.

It intentionally contains no application source code. Only release artifacts are kept here:

- `update.json` — the update manifest the in-app updater verifies (schema version, application id, version, channel, SHA-256, size and the GitHub release download URL).
- `RELEASE-NOTES.md` — the notes shown alongside the latest stable release.
- `*.apk` — release assets attached to GitHub releases (not required to live in the git tree).

Releases are created as drafts, their APK asset is verified (name, size, SHA-256) and only then published. Nothing installs automatically; Android still asks before any installation.
