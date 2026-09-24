Build steps
1. Install Android Studio and open this folder (File > Open). Accept the Gradle sync.
2. Build > Build Bundle(s) / APK(s) > Build APK(s).
3. APK: app/build/outputs/apk/debug/app-debug.apk  (copy to phone and install).
The web app is app/src/main/assets/index.html. Requires Android 10 or newer.
For a release APK use Build > Generate Signed Bundle / APK.

No Android Studio? Build online with GitHub Actions
1. Make a free GitHub account and create a new (private) repository.
2. Upload everything in this folder to the repository root (settings.gradle must be at the top level).
   If the hidden ".github" folder is skipped: Add file > Create new file, name it
   .github/workflows/build.yml and paste the contents of build.yml.txt.
3. Open the Actions tab > "Build APK" > Run workflow (it also runs on upload).
4. When it finishes (about 3-5 minutes), open the run and download "CashFlowTracker-apk" (a zip containing app-debug.apk).
