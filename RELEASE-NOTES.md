# Glow Up 1.3.4 — stable release

## What changed
- Fixed the app hanging on "Opening your journal…": the first secure-storage and photo-signing calls are now time-bounded, so startup ends in the journal or a retry instead of a permanent splash.
- Google sign-in now succeeds even when Android secure storage is unavailable on a device. The session is then kept in memory for that run only, and the app says you will need to sign in again next time.
- Release builds now verify that the signed APK contains the freshly built web bundle, so an update can never ship an older app by mistake.
- Updates the existing glowup.vikashbuilds.in app in place using the same release signature. Keep your installed app; Android asks for confirmation before updating.

## Install or update
1. Download `glowup-1.3.4.apk` from this release.
2. Open it and confirm the Android install or update prompt. Do not uninstall the current `glowup.vikashbuilds.in` app first.
3. Open glowup; your existing signed-in session and journal are retained when updating in place.

## Legacy app
- The old `com.glowup.app` package is separate. Sign in to this app to restore cloud data; export device-only preview entries before removing a legacy build.
