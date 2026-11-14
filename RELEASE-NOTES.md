# Glow Up 1.2.0 — stable release

## New app identity (important)
- This release installs as a **separate app** (`glowup.vikashbuilds.in`, app name "glowup"). It does not upgrade the previous `com.glowup.app` build in place.
- Install it side by side, sign in again inside the new app, then uninstall the old build when you are ready. Your account data lives on the server, so posts and journals come back after sign-in; device-only extras (local reminders, dismissed-notice state) start fresh.
- The APK is signed with Glow Up's private release key. Future updates from this channel must carry the same signature — Android refuses an update signed with a different key.

## What changed
- First stable-channel release under the new application id.
- Carries the 1.1.0 feature set: private-by-default journal entries, daily goals with completions, feed search and topic filters, weekly glow summary, and community encouragement.
- New in-app update notice (startup check plus a manual check in settings) backed by a verified `update.json` manifest: size, SHA-256 and download URL are checked before an update is offered.

## Install
1. Download `glowup-1.2.0.apk` from this release.
2. Open it and confirm the Android install prompt.
3. Sign in with your existing account.
