# Android Profile App

This is a Jetpack Compose Android application that displays a profile card.

## Prerequisites

- Android Studio or Android SDK
- JDK 8 or higher
- Gradle 8.2

## Project Structure

```
Android_mobile_application/
├── app/
│   ├── build.gradle.kts
│   ├── proguard-rules.pro
│   └── src/
│       └── main/
│           ├── AndroidManifest.xml
│           ├── java/com/ahmed/profileapp/
│           │   └── MainActivity.kt
│           └── res/
│               ├── drawable/
│               │   └── README.txt (Add zeyad_photo.png here)
│               ├── mipmap-*/
│               └── values/
│                   ├── strings.xml
│                   └── themes.xml
├── gradle/
│   └── wrapper/
│       └── gradle-wrapper.properties
├── build.gradle.kts
├── settings.gradle.kts
├── gradle.properties
├── gradlew
└── gradlew.bat
```

## Setup Instructions

### 1. Add Profile Photo

Add your profile photo to the drawable folder:
- Place an image file named `zeyad_photo.png` in `app/src/main/res/drawable/`

### 2. Add App Icons (Optional)

For a complete setup, add launcher icons:
- Generate icons at https://romannurik.github.io/AndroidAssetStudio/
- Place them in the appropriate mipmap folders (mipmap-hdpi, mipmap-mdpi, etc.)

### 3. Build the Project

Run the following command to build the project:

```bash
./gradlew build
```

### 4. Run on Android Device/Emulator

#### Using Android Studio:
1. Open this project in Android Studio
2. Connect an Android device or start an emulator
3. Click the "Run" button

#### Using Command Line:
```bash
./gradlew installDebug
```

## Features

- Profile card with circular photo
- Material Design 3 components
- Custom color theme
- Contact button with toast notification
- Email and phone icons

## Requirements

- Minimum SDK: 24 (Android 7.0)
- Target SDK: 34 (Android 14)
- Kotlin version: 1.9.10
- Jetpack Compose BOM: 2023.10.01

## Troubleshooting

If you encounter build errors:
1. Ensure you have the Android SDK installed
2. Make sure ANDROID_HOME environment variable is set
3. Add the profile photo (`zeyad_photo.png`) to the drawable folder
4. Run `./gradlew clean build`
