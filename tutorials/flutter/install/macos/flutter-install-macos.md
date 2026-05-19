[Tutorials](../../../tutorials.md) > [Flutter](../../flutter.md) > [Flutter Install](../flutter-install.md) > Flutter Install macOS

# Flutter Install macOS

## Requirements

- [Android Studio](./../../../android-studio/install/macos/android-studio-install-macos.md)
- [CocoaPods](./../../../cocoapods/install/macos/cocoapods-install-macos.md)
- [Homebrew](./../../../homebrew/install/macos/homebrew-install-macos.md)
- [Xcode Command Line Tools](./../../../xcode-command-line-tools/install/macos/xcode-command-line-tools-install-macos.md)

## Install

```bash
brew install --cask flutter
```

## Configure Flutter Android SDK Location

```bash
flutter config --android-sdk ~/Library/Android/sdk
```

## Accept Android Licenses

```bash
flutter doctor --android-licenses
```

## Check Doctor

```bash
flutter doctor
```

## Check Location

```bash
which flutter
which dart
```

should be something like

```text
/opt/homebrew/bin/flutter
/opt/homebrew/bin/dart
```
