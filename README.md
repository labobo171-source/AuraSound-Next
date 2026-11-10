# AuraSound Ultra 3D Player

A Persian, neon-themed Android music player built with Android WebView.

## Features
- Five visual themes: Neon, Cyberpunk, Galaxy, Matrix and Gold
- Automatic local audio-library scan after the required Android audio permission is granted
- Favorite heart on each track and a persistent Favorites library
- Playlist sorting by name, file size, date and folder
- Playback controls, seek bar, shuffle and repeat
- Native foreground media playback service with Android MediaSession, lock-screen controls and playback notification
- Web Audio processing: amplifier, bass, treble and 10-band equalizer
- Circular audio visualizer and Three.js particle background
- Large-button driving mode

## Build
GitHub Actions builds a debug APK on every push to `main` and on manual workflow dispatch.

1. Open the **Actions** tab.
2. Select **Android APK**.
3. Open the latest successful run.
4. Download **AuraSound-Next-debug-apk** from Artifacts and extract the ZIP.
5. Install `app-debug.apk` on your Android device.

## Notes
- Internet access is used to load Three.js and Font Awesome from their public CDNs.
- Android prompts for audio-library permission; once granted, the app queries the device media library automatically.
- The Android foreground service publishes a MediaSession and media notification for background playback and lock-screen controls.
- This is a debug APK, not a Play Store-signed release.