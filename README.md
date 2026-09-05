# CPAP CSV Exporter - Android App

A modern Android application for importing data from CPAP machines and converting it to CSV files for analysis.

## 📋 Features

- ✅ Material Design 3 UI with Jetpack Compose
- ✅ Modern Android development practices
- ✅ File import and CSV export functionality
- ✅ Android 8.0+ (API level 26) support
- ✅ Data backup and extraction rules
- ✅ Gradle build automation

## 🛠️ Tech Stack

- **Language:** Kotlin
- **UI Framework:** Jetpack Compose
- **Design System:** Material Design 3
- **Min SDK:** 26 (Android 8.0)
- **Target SDK:** 34 (Android 14)
- **Build System:** Gradle 8.0

## 📦 Dependencies

- AndroidX Core KTX 1.12.0
- Lifecycle Runtime KTX 2.6.2
- Activity Compose 1.8.0
- Compose Material3
- Compose UI & Graphics
- JUnit 4 (Testing)
- Espresso (UI Testing)

## 🏗️ Project Structure

```
CPAP-data-exporter-APK/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/example/cpapcsvexporter/
│   │   │   │   ├── MainActivity.kt
│   │   │   │   └── ui/theme/
│   │   │   │       ├── Theme.kt
│   │   │   │       ├── Color.kt
│   │   │   │       └── Type.kt
│   │   │   ├── res/
│   │   │   │   ├── values/
│   │   │   │   │   ├── strings.xml
│   │   │   │   │   └── themes.xml
│   │   │   │   └── xml/
│   │   │   │       ├── backup_rules.xml
│   │   │   │       └── data_extraction_rules.xml
│   │   │   └── AndroidManifest.xml
│   │   ├── test/
│   │   └── androidTest/
│   ├── build.gradle.kts
│   └── proguard-rules.pro
├── gradle/wrapper/
│   └── gradle-wrapper.properties
├── build.gradle.kts
├── settings.gradle.kts
├── gradle.properties
├── gradlew
├── BUILD.md
└── README.md
```

## 🚀 Getting Started

### Prerequisites

- Java Development Kit (JDK) 17 or higher
- Android SDK (API level 34 or higher)
- Gradle 8.0+ (included via gradlew)

### Building

#### Release Build
```bash
./gradlew assembleRelease
```

Output: `app/build/outputs/apk/release/app-release.apk`

#### Debug Build
```bash
./gradlew assembleDebug
```

Output: `app/build/outputs/apk/debug/app-debug.apk`

#### Clean Build
```bash
./gradlew clean assembleRelease
```

## 🔧 Configuration

All build configurations are in `app/build.gradle.kts`:
- **App ID:** com.example.cpapcsvexporter
- **Version:** 0.2
- **Compose Support:** Enabled with Kotlin Compiler Extension 1.5.3

See [BUILD.md](./BUILD.md) for detailed build instructions.

## 📝 Permissions

The app requires the following permissions (from `AndroidManifest.xml`):
- `android.permission.READ_EXTERNAL_STORAGE` - Read CPAP data files
- `android.permission.WRITE_EXTERNAL_STORAGE` - Export CSV files
- `android.permission.INTERNET` - Network connectivity (if needed)

## 🔐 Security

- Data extraction rules configured in `data_extraction_rules.xml`
- Backup rules configured in `backup_rules.xml`
- ProGuard optimization enabled for release builds

## 🧪 Testing

Run tests with:
```bash
./gradlew test
./gradlew connectedAndroidTest
```

## 🎯 Roadmap

- [ ] Implement CPAP data import functionality
- [ ] Add CSV export feature
- [ ] Create data analysis screens
- [ ] Add file management UI
- [ ] Implement data visualization
- [ ] Add user preferences/settings

## 📄 License

This project was created with assistance from ChatGPT to import and analyze CPAP machine data.

## 👨‍💻 Author

Created by bryoung2018-max

## 🤝 Contributing

Feel free to fork and submit pull requests with improvements!

## ⚠️ Note

This is an Android app project extracted and organized from a ZIP file. Some features may still need implementation based on your requirements.

---

**Last Updated:** September 5, 2026
