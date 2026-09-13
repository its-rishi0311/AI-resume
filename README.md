# ElevateCV Android APK

This project packages the supplied ElevateCV PWA as a standalone Android app using Capacitor.

## Build locally

Requirements: Node.js 20+, Android Studio/Android SDK, and a JDK compatible with your installed Android Gradle Plugin.

```bash
npm install
npx cap add android
npx cap sync android
cd android
./gradlew assembleDebug
```

APK output:

`android/app/build/outputs/apk/debug/app-debug.apk`

## Build APK automatically with GitHub Actions

Push this repository to GitHub, then open **Actions → Build Android APK → Run workflow**. The workflow builds the debug APK and uploads it as a downloadable artifact.

The supplied web app, service worker, manifest, and app icon are kept in `www/`.
