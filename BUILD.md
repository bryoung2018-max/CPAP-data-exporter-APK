# CPAP CSV Exporter - Build Instructions

## Prerequisites
- Java Development Kit (JDK) 17 or higher
- Android SDK with API level 34
- Gradle 8.0 or higher (included via gradlew)

## Building the APK

### Release Build
```bash
./gradlew assembleRelease
```

The release APK will be generated at:
```
app/build/outputs/apk/release/app-release.apk
```

### Debug Build
```bash
./gradlew assembleDebug
```

The debug APK will be generated at:
```
app/build/outputs/apk/debug/app-debug.apk
```

### Clean Build
```bash
./gradlew clean assembleRelease
```

## Project Information

- **App Name:** CPAP CSV Exporter
- **Version:** 0.2
- **Min SDK:** 26 (Android 8.0)
- **Target SDK:** 34 (Android 14)
- **Package Name:** com.example.cpapcsvexporter

## Key Dependencies

- AndroidX Core KTX 1.12.0
- Compose Material3
- Jetpack Compose 2023.10.00
- JUnit 4.13.2
- Espresso 3.5.1

## Build Features

- ✅ Jetpack Compose UI
- ✅ Material Design 3
- ✅ Android X compatibility
- ✅ ProGuard optimization

## GitHub Actions Workflow

To enable automated builds, create `.github/workflows/build-apk.yml` with the following workflow configuration. Due to permission restrictions, this file needs to be created manually or through the GitHub web interface.

See the repository for workflow setup details.
