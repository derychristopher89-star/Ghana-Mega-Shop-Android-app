# Ghana Mega Shop Android project

This Android Studio project wraps the currently published Ghana Mega Shop website in an Android WebView.

- App name: Ghana Mega Shop
- Application ID: `com.ghanamegashop.app`
- Website: https://derychristopher89-star.github.io/Ghana-mega-shop/
- WhatsApp ordering is handled by the website and opens WhatsApp/browser as appropriate.

## Important limitations

The project targets Android 16 (API 36), which is required for new Google Play submissions from 31 August 2026.

This is a starter wrapper project, not a finished commercial app. It does not add native product management, payment processing, or a central order database. The current website says its product listings are samples, so replace them with real stock/prices before accepting orders. Google Play review is not guaranteed; a minimal website wrapper may fail its functionality/quality policies. Test all flows and review current Play Console policies before submitting.

## Build using GitHub Actions from your phone

1. Create a new public GitHub repository, e.g. `ghana-mega-shop-android`.
2. Upload the extracted contents of this project ZIP to the repository root.
3. Open the repository's **Actions** tab and enable Actions if prompted.
4. Select **Build Ghana Mega Shop Android app** and tap **Run workflow** (or push a commit to `main`).
5. When the workflow completes, open the run and download the artifact named `ghana-mega-shop-android-builds`.

The artifact contains a debug APK for testing and an **unsigned release AAB**. The unsigned AAB is not ready for Google Play. Before Play submission, the release must be signed with a secure upload key and configured in Play Console. Never share your keystore or passwords in chat or commit them to GitHub.

## Build locally

Open this folder in Android Studio, let Gradle sync, then use Build > Build Bundle(s) / APK(s). For Google Play, configure release signing securely before building the final AAB.
