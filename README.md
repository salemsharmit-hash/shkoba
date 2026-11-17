# Shkoba (Chkobba)

Web app (GitHub Pages) + phone apps via Capacitor 8.

- Web: `index.html` (installable PWA, works offline)
- Android: `android/` — the "Build Android app" GitHub Action produces a debug APK (Actions → latest run → Artifacts)
- iOS: `ios/` — Swift Package Manager (no CocoaPods needed). On a Mac with Xcode:
  1. `npm ci && npm run sync`
  2. `npx cap open ios` (or open `ios/App/App.xcodeproj`)
  3. In Xcode: target App → Signing & Capabilities → pick your Team (Apple ID), then press Run with your iPhone selected.
- After changing the web files run `npm run sync` to copy them into both phone projects.
