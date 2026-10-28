# Build JARVIS APK using only an Android phone

This project is a starter app, not a finished AI assistant. The workflow builds a debug APK in GitHub Actions.

## Phone-only outline
1. Download and extract this ZIP using your phone's file manager.
2. In a browser, create a new GitHub repository named `jarvis-android` (a public repository is simplest for GitHub Actions free usage; don't upload passwords, API keys, or private data).
3. Upload the *contents* of the extracted project to the repository's `main` branch, preserving folder paths. Make sure `.github/workflows/build.yml` is included. If GitHub's mobile upload interface doesn't let you upload folders, use GitHub's web editor to create the files/folders or use a browser's desktop-site mode.
4. Open the repository's **Actions** tab, select **Build JARVIS APK**, then **Run workflow** if it has not started automatically.
5. Open the completed run, scroll to **Artifacts**, and download `JARVIS-debug-APK`. Extract the downloaded artifact ZIP to get the `.apk`.
6. Tap the APK to install. Android may ask you to allow installation from that browser/file manager; only allow it for the file you just built and trust.

## Important
- The APK is a debug build, intended for testing.
- The app currently has a basic interface, a scheduled notification, and an in-app simulated call screen. It does not yet include a connected AI model, speech recognition/TTS, real phone calls, or guaranteed alarm-like behavior.
- The project may need fixes if the cloud build reports a compile error. Don't add API keys or passwords to a public repository.
