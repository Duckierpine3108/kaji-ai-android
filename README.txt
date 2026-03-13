KAJI AI v7 - Android APK
by Kamran Jalil Khan - ProsperaOS, Pakistan
============================================

HOW TO BUILD YOUR APK (No Android Studio needed)
-------------------------------------------------

STEP 1 - Create a free GitHub account
  Go to: https://github.com
  Sign up for free

STEP 2 - Create a new repository
  Click the + button (top right) > New repository
  Name it: kaji-ai-android
  Set it to: Public
  Click: Create repository

STEP 3 - Upload this entire folder
  On your new repo page, click "uploading an existing file"
  Drag and drop ALL files and folders from this kaji-android folder
  (including the hidden .github folder - make sure to include it!)
  Scroll down, click "Commit changes"

STEP 4 - Watch it build automatically
  Click the "Actions" tab at the top of your repo
  You will see "Build KAJI AI APK" running
  Wait 5-10 minutes for it to finish
  When it shows a green checkmark - it is done!

STEP 5 - Download your APK
  Click on the completed workflow run
  Scroll down to "Artifacts"
  Click "KAJI-AI-v7-APK" to download
  Extract the ZIP - inside is your app-debug.apk

STEP 6 - Install on your Android phone
  Copy app-debug.apk to your phone
  Go to Settings > Security > Allow unknown sources (or Install unknown apps)
  Open the APK file on your phone
  Tap Install
  Done! KAJI AI is now on your phone.

============================================

WHAT THIS APP INCLUDES
- Full KAJI AI v7 with all features
- DeepSeek R1 as the default AI (powerful reasoning model)
- Cinematic 10-second splash screen
- Full screen mode (no browser bar)
- Home screen icon: KAJI AI
- Works on Android 5.1 and above
- Offline mode: shows cached chats when no internet

============================================

TROUBLESHOOTING

Build fails with "gradle wrapper" error:
  - Delete the file android/gradle/wrapper/gradle-wrapper.jar
  - Go to Actions tab > click the failed run > Re-run jobs

"Unknown sources" not showing on phone:
  - Samsung: Settings > Biometrics and security > Install unknown apps
  - Xiaomi/Redmi: Settings > Privacy > Special app access > Install unknown apps
  - General: Settings > Apps > Special app access > Install unknown apps

APK installs but app crashes:
  - Make sure you have internet connection on first launch
  - Try clearing app data: Settings > Apps > KAJI AI > Clear data

============================================

FOLDER STRUCTURE

kaji-android/
  .github/
    workflows/
      build-apk.yml        - GitHub Actions build script (DO NOT EDIT)
  android/
    app/
      src/main/
        assets/www/
          index.html       - KAJI AI full app (the brain)
        java/.../
          MainActivity.java - Android activity
        res/
          mipmap-*/        - App icons (all sizes)
          values/          - Strings, styles, themes
        AndroidManifest.xml - App permissions and config
      build.gradle         - App build config
    build.gradle           - Project build config
    settings.gradle        - Project settings
    gradle.properties      - Gradle settings
    gradlew                - Build script
    gradle/wrapper/        - Gradle wrapper files
  capacitor.config.json    - Capacitor config
  package.json             - Project info
  README.txt               - This file

============================================
KAJI AI (c) 2026 Kamran Jalil Khan - ProsperaOS
