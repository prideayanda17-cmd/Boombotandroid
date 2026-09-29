# BoomBot Android Controller — Cloud Build

This project is the Android controller prototype for the Boom 1000 MT5 robot.

## Important
The current Android app is a controller/dashboard prototype. Its Start/Stop buttons do not yet execute trades or control MT5 remotely. The MT5 Expert Advisor remains responsible for actual trading.

## Build the APK from a phone
1. Create a free GitHub account at github.com if you do not already have one.
2. Create a new empty repository, for example `BoomBotAndroid`.
3. Extract this ZIP on your Android phone.
4. Upload the extracted project files to the GitHub repository.
5. Make sure `.github/workflows/build-apk.yml` is included.
6. Open the repository's **Actions** tab.
7. Select **Build BoomBot Android APK** and run the workflow if it did not start automatically.
8. When the build finishes, open the workflow run and download the **BoomBot-debug-apk** artifact.
9. Extract the downloaded artifact and install the APK on your Android phone.

## If GitHub mobile upload hides .github
You can create the workflow directly in GitHub:
- New file path: `.github/workflows/build-apk.yml`
- Paste the contents of the included `build-apk.yml` file.
- Commit it to the `main` branch.

The workflow uses Android Gradle Plugin 8.7.x with Gradle 8.9 compatibility.
