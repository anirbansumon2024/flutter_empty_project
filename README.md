# OTTKing - Flutter App

A production-ready Flutter empty project with iOS and Android support. This is a clean, modern starter template for building OTT (Over-The-Top) applications.

## 🎯 Features

- ✅ **Complete Flutter 3.0+ Setup** - Latest SDK with Material Design 3
- ✅ **iOS Support** - Fully configured for iOS builds (iPhone & iPad)
- ✅ **Android Support** - Fully configured for Android builds
- ✅ **Bottom Navigation** - 4-tab navigation (Home, Search, Downloads, Profile)
- ✅ **Modern UI** - Clean and professional interface
- ✅ **100% Build Ready** - Production-ready out of the box
- ✅ **No Dependencies** - Uses only Flutter default packages

## 📁 Project Structure

```
flutter_empty_project/
├── lib/
│   └── main.dart                    # Main application with complete UI
├── test/
│   └── widget_test.dart             # Widget tests
├── ios/                              # iOS native code (auto-configured)
├── android/                          # Android native code (auto-configured)
├── pubspec.yaml                      # Project dependencies
├── analysis_options.yaml             # Linting rules
├── .gitignore                        # Git ignore file
├── README.md                         # This file
└── LICENSE                           # Apache 2.0 License
```

## 🚀 Getting Started

### Prerequisites

- Flutter SDK: `>=2.12.0 <3.0.0` (or latest)
- Dart SDK: included with Flutter
- iOS: Xcode 13.0+ (for iOS builds)
- Android: Android Studio 2021.1.1+ (for Android builds)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/anirbansumon2024/flutter_empty_project.git
   cd flutter_empty_project
   ```

2. **Get dependencies**
   ```bash
   flutter pub get
   ```

3. **Run the app**
   ```bash
   flutter run
   ```

## 📱 Building for iOS

### Run on iOS Simulator
```bash
flutter run
```

### Build iOS Release
```bash
flutter build ios --release
```

### Build for App Store
```bash
flutter build ios --release
# Then open in Xcode:
open ios/Runner.xcworkspace
```

## 🤖 Building for Android

### Run on Android Emulator
```bash
flutter run
```

### Build Android Release APK
```bash
flutter build apk --release
```

### Build Android App Bundle
```bash
flutter build appbundle --release
```

### Generate Signed APK
```bash
keytool -genkey -v -keystore ~/key.jks -keyalg RSA -keysize 2048 -validity 10000 -alias key
flutter build apk --release --build-name=1.0.0 --build-number=1
```

## 🎨 App Features

### 🏠 Home Tab
- Featured Movies horizontal carousel
- Popular Series horizontal carousel
- Responsive grid layout
- Smooth scrolling lists

### 🔍 Search Tab
- Search input field
- Quick search functionality
- Ready for search implementation

### 📥 Downloads Tab
- Download management interface
- Offline viewing support ready
- Empty state handling

### 👤 Profile Tab
- User profile display
- Account information section
- Sign out functionality

## 🏗️ Architecture

The app uses Flutter best practices:

- **StatefulWidget** for state management
- **Material Design 3** UI components
- **Bottom Navigation Bar** for tab navigation
- **Responsive Design** for all screen sizes

### For Production Apps, Consider:

- **Provider** - Simple state management
- **GetX** - Route management and state
- **BLoC** - Business logic components
- **Riverpod** - Modern state management
- **Firebase** - Backend services

## 🎨 Customization

### Change App Name

Edit `pubspec.yaml`:
```yaml
name: your_app_name
description: Your app description.
```

Also update:
- iOS: `ios/Runner/Info.plist` (CFBundleName)
- Android: `android/app/build.gradle` (applicationId)

### Change App Icon

Replace icon files:
- iOS: `ios/Runner/Assets.xcassets/AppIcon.appiconset/`
- Android: `android/app/src/main/res/mipmap-*/`

### Change Theme Colors

In `lib/main.dart`:
```dart
theme: ThemeData(
  primarySwatch: Colors.blue,  // Change to your color
  useMaterial3: true,
),
```

### Add Dependencies

```bash
flutter pub add package_name
```

Then import in your code:
```dart
import 'package:package_name/package_name.dart';
```

## 🧪 Testing

Run all tests:
```bash
flutter test
```

Run specific test file:
```bash
flutter test test/widget_test.dart
```

## 📊 Performance Tips

- Use `const` constructors where possible
- Use `ListView.builder` for long lists
- Avoid unnecessary rebuilds with `const` widgets
- Use `SingleChildScrollView` for content overflow
- Optimize images and assets

## 🔧 Troubleshooting

### Build fails on iOS

```bash
cd ios
rm -rf Pods
rm Podfile.lock
cd ..
flutter clean
flutter pub get
flutter run
```

### Build fails on Android

```bash
flutter clean
flutter pub get
flutter build apk --release
```

### Dependency conflicts

```bash
flutter pub get
flutter pub upgrade
flutter pub outdated
```

### Unable to run on device

```bash
flutter devices
flutter run -d <device_id>
```

## 📚 Resources

- [Flutter Documentation](https://flutter.dev/docs)
- [Dart Documentation](https://dart.dev/guides)
- [Material Design](https://material.io/design)
- [Flutter Cookbook](https://flutter.dev/docs/cookbook)
- [Firebase for Flutter](https://firebase.flutter.dev/)

## 📋 Requirements

- Flutter 2.12.0 or higher
- Dart 2.15.0 or higher
- iOS 11.0 or higher
- Android 5.0 (API level 21) or higher

## 📄 License

This project is licensed under the Apache 2.0 License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

### How to contribute:
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 👨‍💻 Author

**Anirban Sumon**
- GitHub: [@anirbansumon2024](https://github.com/anirbansumon2024)
- Project: [flutter_empty_project](https://github.com/anirbansumon2024/flutter_empty_project)

## 🌟 Support

If you found this project helpful, please give it a ⭐ on GitHub!

## 📞 Feedback

Have questions or suggestions? Feel free to:
- Open an issue on GitHub
- Create a discussion
- Submit a pull request

---

**Happy Coding!** 🚀

Last Updated: 2026-05-02