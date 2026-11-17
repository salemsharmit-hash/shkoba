# Shkoba (Chkobba)

Web app (GitHub Pages) + phone apps via Capacitor.

- Web: `index.html` (installable PWA, works offline)
- Android: `android/` — the "Build Android app" GitHub Action produces a debug APK (Actions → latest run → Artifacts)
- iOS: `ios/` — needs a Mac with Xcode and an Apple developer account: `npm ci && npm run sync && npx cap open ios`
- After changing the web files run `npm run sync` to copy them into both phone projects.
