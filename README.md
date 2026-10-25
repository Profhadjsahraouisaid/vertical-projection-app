# الإسقاط العمودي — Android app

This Android WebView project packages the supplied Arabic HTML lesson as an installable APK. The lesson's interactive canvas and JavaScript are kept in `app/src/main/assets/index.html`.

## Build an APK using GitHub on your phone

1. Download and unzip this project ZIP.
2. Open GitHub in your phone browser and create a **public or private** repository (for example, `projection-app`).
3. Open the new repository, choose **Add file → Upload files**, and upload the **contents** of this folder (including `.github`, `app`, `build.gradle`, `settings.gradle`, and `gradle.properties`). If `.github` is hidden by your file manager, make sure the workflow file is uploaded at `.github/workflows/build-apk.yml`.
4. Commit the uploaded files to the `main` branch.
5. Open the repository's **Actions** tab. Choose **Build Android APK** and press **Run workflow** if it has not started automatically.
6. Open the newest workflow run. Wait for the green check mark, then scroll to **Artifacts** and download **ProjectionApp-debug-apk**.
7. Extract the downloaded artifact ZIP to get `app-debug.apk`. Open it on your Android phone and allow installation from that source if Android asks.

## Notes
- This creates a **debug APK** for testing and direct installation, not a Play Store release.
- No internet permission is requested; the HTML lesson is bundled inside the app and can work offline.
- App ID: `com.hadjsahraoui.projection`.
