# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Flutter project named "dday" - a cross-platform mobile application that supports Android, iOS, Web, Windows, macOS, and Linux platforms. The project is currently a standard Flutter template with the default counter app implementation.

## Development Commands

### Running the Application

```bash
# Run on the default device
flutter run

# Run on specific platform
flutter run -d chrome          # Web
flutter run -d macos          # macOS
flutter run -d windows        # Windows
flutter run -d linux          # Linux
```

### Testing

```bash
# Run all tests
flutter test

# Run specific test file
flutter test test/widget_test.dart

# Run tests with coverage
flutter test --coverage
```

### Code Quality

```bash
# Analyze code for issues
flutter analyze

# Format code
flutter format .

# Check for outdated dependencies
flutter pub outdated

# Update dependencies
flutter pub upgrade
```

### Building

```bash
# Build for different platforms
flutter build apk           # Android APK
flutter build appbundle     # Android App Bundle
flutter build ios           # iOS
flutter build web           # Web
flutter build macos         # macOS
flutter build windows       # Windows
flutter build linux         # Linux
```

## Project Structure

- `lib/main.dart` - Main application entry point with MaterialApp setup
- `test/` - Widget and unit tests
- `android/` - Android-specific platform code and configuration
- `ios/` - iOS-specific platform code and configuration
- `web/` - Web-specific assets and configuration
- `windows/` - Windows-specific platform code
- `macos/` - macOS-specific platform code
- `linux/` - Linux-specific platform code

## Code Analysis

The project uses `flutter_lints` for code analysis with rules defined in `analysis_options.yaml`. The linting configuration follows Flutter's recommended practices.

## Dependencies

- **flutter**: Core Flutter framework
- **cupertino_icons**: iOS-style icons
- **flutter_lints**: Development-time linting rules
- **flutter_test**: Testing framework

## Platform Support

This project is configured for all Flutter-supported platforms:

- Android (minSdkVersion and targetSdkVersion configured)
- iOS (deployment target and capabilities configured)
- Web (with Progressive Web App manifest)
- Windows (with CMake build configuration)
- macOS (with Xcode project configuration)
- Linux (with CMake build configuration)
