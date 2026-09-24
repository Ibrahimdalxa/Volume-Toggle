<div align="center">

<img src="icon.png" width="120" height="120" alt="Volume Toggle icon" />

# 🔊 Volume Toggle

**Mute and unmute your phone in one tap. No fumbling with hardware buttons, no digging through settings.**

[![Platform](https://img.shields.io/badge/platform-Android-3DDC84?logo=android&logoColor=white)](https://developer.android.com)
[![Min SDK](https://img.shields.io/badge/minSdk-24%20(Android%207.0+)-blue)](https://developer.android.com/tools/releases/platforms)
[![Built with](https://img.shields.io/badge/UI-Jetpack%20Compose-4285F4?logo=jetpackcompose&logoColor=white)](https://developer.android.com/jetpack/compose)
[![License](https://img.shields.io/badge/license-MIT-lightgrey)](#license)

[Download APK](#-installation) · [Features](#-features) · [Build from Source](#-build-from-source) · [Contribute](#-contributing)

<a href="https://github.com/Ibrahimdalxa/Volume-Toggle/releases/download/v1.0.0/Volume-Toggle.apk">
  <img src="https://img.shields.io/badge/⬇️%20Download-Volume--Toggle.apk-brightgreen?style=for-the-badge" alt="Download APK" />
</a>

</div>

---

## 📖 Overview

**Volume Toggle** is a lightweight Android utility built for one thing: getting your phone silent (or loud again) as fast as physically possible. Instead of pressing the volume rocker a dozen times or diving into the notification shade, Volume Toggle gives you a single, satisfying switch that flips your device between sound and silence instantly.

It's built entirely with modern Android tooling — Kotlin, Jetpack Compose, and Material 3 — so it feels right at home on any recent version of Android while staying fast and battery-friendly.

## ✨ Features

- **One-tap mute/unmute** — A single switch instantly toggles your device's ringer mode between normal and silent.
- **Home screen widget** — Drop the toggle right on your home screen for access without even opening the app.
- **Clean Material 3 interface** — Built with Jetpack Compose for a smooth, modern look that adapts to your system theme (including dynamic color / dark mode).
- **Instant state sync** — The toggle always reflects your phone's real, current volume state — no stale UI.
- **Lightweight & fast** — No bloat, no unnecessary background services eating your battery.

> Have a feature request? Open an issue — see [Contributing](#-contributing) below.

## 📱 Screenshots

<div align="center">

| Home Screen | Mute Toggled | Toggle Off |
|:---:|:---:|:---:|
| <img src="https://i.ibb.co.com/7JJwhwMK/home-screen.jpg" width="200" /> | <img src="https://i.ibb.co.com/4R5C6WgF/mute.jpg" width="200" /> | <img src="https://i.ibb.co.com/B2fMx69f/toggle-off.jpg" width="200" /> |

</div>

## 📥 Installation

### Option 1 — Download the APK (recommended for most users)

1. Tap the **[⬇️ Download Volume-Toggle.apk](https://github.com/Ibrahimdalxa/Volume-Toggle/releases/download/v1.0.0/Volume-Toggle.apk)** button above, or grab it from the [Releases](https://github.com/Ibrahimdalxa/Volume-Toggle/releases) page.
2. On your Android device, open the downloaded file. If prompted, allow installation from this source (**Settings → Security → Install unknown apps**).
3. Tap **Install**, then open the app and start toggling.

> **Note:** Since this build isn't distributed through the Google Play Store, some devices (especially Honor/Huawei) will show an "unverified app" warning — this is expected for sideloaded APKs. Review the source code here if you'd like to verify what's inside before installing.

### Option 2 — Build it yourself

See [Build from Source](#-build-from-source) below.

## 🛠 Build from Source

**Requirements:**
- [Android Studio](https://developer.android.com/studio) (latest stable)
- JDK 17+
- Android SDK with `compileSdk 36` installed

**Steps:**

```bash
# Clone the repository
git clone https://github.com/Ibrahimdalxa/Volume-Toggle.git
cd Volume-Toggle

# Open in Android Studio and let Gradle sync, or build from the CLI:
./gradlew assembleDebug

# The output APK will be at:
# app/build/outputs/apk/debug/app-debug.apk
```

To build a signed release APK, configure your own signing key in `app/build.gradle` and run:

```bash
./gradlew assembleRelease
```

## 🧱 Tech Stack

| Layer | Technology |
|---|---|
| Language | Kotlin |
| UI | Jetpack Compose + Material 3 |
| Architecture | MVVM |
| Local storage | Jetpack DataStore (Preferences) |
| Database | Room |
| Dependency Injection | Dagger |
| Async | Kotlin Coroutines |

## 🔒 Permissions

| Permission | Why it's needed |
|---|---|
| `ACCESS_NOTIFICATION_POLICY` | Required by Android to programmatically change the device's ringer/silent mode (Do Not Disturb access). |
| `ACCESS_NETWORK_STATE` / `INTERNET` | Used by underlying Google Play services libraries bundled with the app. |

Volume Toggle does **not** collect, transmit, or sell any personal data.

## 📋 Requirements

- **Minimum Android version:** Android 7.0 (API 24) and above
- **Architectures supported:** `arm64-v8a`, `armeabi-v7a`, `x86`, `x86_64`

## 🤝 Contributing

Contributions, bug reports, and feature ideas are all welcome!

1. Fork the repo
2. Create a feature branch (`git checkout -b feature/my-feature`)
3. Commit your changes
4. Open a pull request

If you just want to report a bug, [open an issue](https://github.com/Ibrahimdalxa/Volume-Toggle/issues) with steps to reproduce and your device/Android version.

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

<div align="center">
Made with ❤️ for people tired of hunting for the mute button.
</div>
