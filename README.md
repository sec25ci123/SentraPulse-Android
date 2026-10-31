# SentraPulse Android wrapper

This Android project opens the hosted SentraPulse Streamlit app in a WebView.

## Build APK using GitHub Actions (phone-friendly)

1. Create a GitHub repository named `SentraPulse-Android`.
2. Upload all files and folders from this project to the repository root.
3. Open the repository's **Actions** tab.
4. Select **Build SentraPulse APK**.
5. Tap **Run workflow** (or wait for the push-triggered build).
6. Open the completed workflow run.
7. Under **Artifacts**, download `SentraPulse-Android-APK`.
8. Extract the ZIP and install `app-debug.apk` on your Android phone.

If GitHub asks, enable Actions for the repository.

## Notes

- The APK is a WebView wrapper, not a standalone/offline AI model.
- Internet is required because AI inference and the Streamlit app run on the hosted server.
- The app requests Android camera permission for live camera use.
- Image/video selection uses Android's system file picker.
- Live WebRTC camera support depends on the phone's WebView, browser media support, network, and Streamlit WebRTC connectivity.
- This is a debug APK for testing. A release APK should be signed before public distribution.
