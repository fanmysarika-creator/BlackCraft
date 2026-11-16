# BlackCraft — Android (Capacitor 8)

Файлы игры (index.html, manifest.webmanifest, sw.js, три иконки) — оригинальные, без изменений.
APK собирает GitHub Actions: `npm install` → `prepare_android.py web` → `npx cap add android` →
`prepare_android.py native` → `npx cap sync` → `./gradlew assembleDebug`.

Версии: Capacitor ~8.0.0, minSdk 24, compile/target SDK 36, AGP 8.13.0, Gradle 8.14.3, JDK 21 (Temurin), Node 22.

Файл `build.yml` должен лежать в `.github/workflows/build.yml` (на телефоне: открыть файл на GitHub →
карандаш → в поле имени вписать `.github/workflows/build.yml` → Commit).
Запуск: вкладка Actions → «Сборка BlackCraft APK» → Run workflow. APK: внизу страницы запуска, Artifacts → BlackCraft-APK.
