# Android port status — CRIMSON Launcher

**Status: not yet a working Android APK.** This source archive is a branding/source baseline, not a finished mobile port. No APK has been built or device-tested from this fork.

The uploaded 2.8.1 archive contains Android launcher icon resources under `src-tauri/icons/android/`, but it does not contain a generated Tauri Android project (`src-tauri/gen/android`), Gradle wrapper/project, Android manifest, or Android-specific Rust integration. Icon assets alone do not make an Android application.

Before Android can be called supported, the following engineering work is required:

1. Generate and configure the Tauri Android project and Gradle build.
2. Audit every Rust dependency and platform module for `target_os = \"android\"` support; desktop-only tray, autostart, window, and process APIs must be gated or replaced.
3. Port the game runtime/graphics launch path to Android. A desktop JVM child-process launcher is not automatically compatible with Android's app/runtime and graphics model.
4. Replace Millida-only account, cloud, social, skin, hosting, updater, telemetry, and proxy services with CRIMSON-owned services or disable those functions with clear UI states. The upstream trademark policy explicitly requires a fork to use its own keys and endpoints.
5. Register CRIMSON's own Microsoft Entra app and Discord application before enabling those integrations. Never ship the upstream app IDs or signing keys.
6. Build and test on real ARM64 Android devices across supported Android versions, Minecraft versions, Java runtimes, and loaders.

Until those steps are completed, do not describe this archive as Android-compatible or distribute it as a working APK.
