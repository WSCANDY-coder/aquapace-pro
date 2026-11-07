# AquaPace Pro — Mobile Distance Swimming Pace App

AquaPace Pro is an offline-capable mobile app tailored specifically for competitive age-group swimmers (All Competitive Strokes (Free, Back, Breast, Fly, IM) from 50m to 1500m) and swim coaches.

---

## 📱 How to Run as a Standalone App on Android & Apple

### 🟢 Android (Standalone `.apk` & App Store)

You have three straightforward options for Android:

#### Option 1: Automatic Cloud Build (No Android Studio or SDK required)
1. Push this project to GitHub.
2. The included GitHub Action (`.github/workflows/build-apk.yml`) automatically builds the standalone `AquaPace-Pro.apk`.
3. Go to the **Actions** tab on GitHub, click on the latest build, and download `AquaPace-Pro-Android-APK`.
4. Copy the `.apk` to any Android phone or tap the download link directly on the phone to install!

#### Option 2: 1-Click APK via PWABuilder (Official Microsoft / Google Tool)
1. Deploy your app to Netlify Drop or GitHub Pages (takes 30 seconds).
2. Go to [pwabuilder.com](https://www.pwabuilder.com/) and paste your link.
3. Click **Package for Stores** $\rightarrow$ **Android**.
4. Download your signed Google Play package or direct `.apk`.

#### Option 3: Local Android Studio
1. Open the [`aquapace/android`](file:///c:/Users/andre/Squad%20time%20Gap/aquapace/android) folder in Android Studio.
2. Click **Build $\rightarrow$ Build Bundle(s) / APK(s) $\rightarrow$ Build APK(s)**.
3. The `.apk` will be generated in `app/build/outputs/apk/debug/app-debug.apk`.

---

### 🍎 Apple (iOS / iPhone)

Apple has different rules for standalone apps:

#### Option 1: The Instant Standalone PWA (Free & No App Store Wait)
Because Apple restricts sideloading `.ipa` files directly, Apple's official zero-cost method for standalone apps is:
1. Open your link in **Safari**.
2. Tap the **Share** button (<svg width="12" height="12" style="display:inline" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8.684 13.342C8.886 12.938 9 12.482 9 12c0-.482-.114-.938-.316-1.342m0 2.684a3 3 0 110-2.684m0 2.684l6.632 3.316m-6.632-6l6.632-3.316m0 0a3 3 0 105.367-2.684 3 3 0 00-5.367 2.684zm0 9.316a3 3 0 105.368 2.684 3 3 0 00-5.368-2.684z"/></svg>).
3. Tap **"Add to Home Screen"** (➕).
4. Tap **Add**.
5. Once added, iOS runs it in **standalone mode**:
   - Gets its own home screen icon.
   - Runs full-screen with no Safari browser bars.
   - Stores data in its own private storage sandbox.
   - Works 100% offline at poolside.

#### Option 2: Apple App Store / TestFlight (Requires $99/year Apple Developer Account)
If your swim club or team wants it listed in the official App Store or distributed via TestFlight:
1. Paste your URL into [pwabuilder.com](https://www.pwabuilder.com/) and choose **Package for Stores $\rightarrow$ iOS**.
2. PWABuilder generates an Xcode project ready for signing and upload to Apple App Store Connect / TestFlight.

---

## 🏊 Poolside Features for Swimmers

- **100% Offline Natatorium Mode**: Works without internet or cellular signal in pool basements.
- **Screen Wake Lock**: Keeps the phone screen from sleeping while resting on a kickboard.
- **County Standards Database**: Preloaded qualifying benchmarks across age bands (11/12 up to 17+ Senior) for 25m and 50m pools.
- **One-Tap Share**: Send splits via WhatsApp, iMessage, AirDrop, or Notes.
- **Saved Swimmer Profiles**: Save specific target race plans for individual athletes.
