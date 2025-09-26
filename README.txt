Philips 432 Szimulátor - Android Projektváz

Ez a csomag tartalmazza:
- www/index.html (színes UI + hibakód szimuláció menüvel)
- .github/workflows/android-build.yml (CI workflow)

APK build (helyben):
1. Nyisd meg a projektet parancssorban.
2. Futtasd: npm init -y
3. npm install @capacitor/core @capacitor/cli
4. npx cap init philips432 hu.openai.philips432 --web-dir=www
5. npx cap add android
6. npx cap sync android
7. npx cap open android (Android Studio)
8. Build APK

Automatikus build GitHub Actions segítségével:
- Használd a mellékelt .github/workflows/android-build.yml fájlt.
- Push után a CI legyártja a debug APK-t artifactként.
