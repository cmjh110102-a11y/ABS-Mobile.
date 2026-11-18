# ABS Mobile Android Prototype

Android native starter project for a baseball ABS camera app.

## Prototype included
- CameraX live preview (rear camera)
- Landscape fullscreen broadcast-inspired UI
- Strike zone overlay
- Calibration toggle and drag-to-position zone
- BALL / STRIKE buttons and basic count display

## Not yet included
- Actual AI ball detector / object tracking model
- Automated pitch trajectory analysis
- Camera-to-field geometry and 3D calibration
- Automatic BALL/STRIKE inference. The buttons are manual demo controls.

## Build APK
Open this folder in Android Studio, allow Gradle sync, then choose **Build > Build APK(s)**.
Requires Android Studio and Android SDK (compile SDK 35). The APK will be in `app/build/outputs/apk/debug/` after build.

## Build APK with GitHub Actions (cloud build)

1. Upload this project to a GitHub repository (the repository root should contain `settings.gradle`, `build.gradle`, and `app/`).
2. Open **Actions** → **Build ABS Mobile APK** → **Run workflow**.
3. Wait for the workflow to finish successfully.
4. Open the completed workflow run and download the artifact named **ABS-Mobile-debug-apk**. It contains `app-debug.apk`.
5. Transfer `app-debug.apk` to your Android phone and install it. If prompted, allow installing apps from that source.

This produces a debug APK for testing; it is not a Play Store release build.
