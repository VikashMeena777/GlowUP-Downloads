# Glow Up 1.3.5 — stable release

## What changed
- Fixed the real cause of signing in on every launch: loading the native secure-storage plugin returned a thenable object, so JavaScript called a non-existent native method and every storage call reported "unavailable". Sessions are now saved in the Android Keystore and restored when you reopen the app - stay signed in until you sign out.
- Fixed the same plugin-loading defect for app resume, so journal and community data refresh when you come back to the app instead of staying stale.
- Start-up remains bounded (about one second to the journal on a mid-range phone) and a memory-only fallback still exists for devices whose secure storage genuinely fails, instead of blocking sign-in.
- Release builds now verify that the signed APK contains the freshly built web bundle, so an update can never ship an older app by mistake.
- Updates the existing glowup.vikashbuilds.in app in place using the same release signature. Keep your installed app; Android asks for confirmation before updating.

## Install or update
1. Download `glowup-1.3.5.apk` from this release.
2. Open it and confirm the Android install or update prompt. Do not uninstall the current `glowup.vikashbuilds.in` app first.
3. Open glowup; your existing signed-in session and journal are retained when updating in place.

## Legacy app
- The old `com.glowup.app` package is separate. Sign in to this app to restore cloud data; export device-only preview entries before removing a legacy build.
