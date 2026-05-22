# Multiplex Android TV packaging

This directory contains an Android TV application scaffold for packaging Multiplex as an Android app target.

## Requirements

- Android Studio (latest stable) or Android SDK + Gradle
- Android TV emulator or device (API 23+)

## Build

From the `android-tv` directory:

```sh
./gradlew :app:assembleDebug
```

If you don't use the Gradle wrapper, run with your local Gradle installation:

```sh
gradle :app:assembleDebug
```

The resulting debug APK is created at:

`app/build/outputs/apk/debug/app-debug.apk`

## Run

Install to an Android TV emulator/device:

```sh
adb install -r app/build/outputs/apk/debug/app-debug.apk
```

