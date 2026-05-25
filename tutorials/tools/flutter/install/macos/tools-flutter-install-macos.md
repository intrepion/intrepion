[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [Flutter](../../tools-flutter.md) > [Install](../tools-flutter-install.md) > macOS

# Tools Flutter Install macOS

## Requirements

- [Android Studio](../../../android-studio/install/macos/tools-android-studio-install-macos.md)
- [CocoaPods](../../../cocoapods/install/macos/tools-cocoapods-install-macos.md)
- [Homebrew](../../../homebrew/install/macos/tools-homebrew-install-macos.md)
- [Xcode Command Line Tools](../../../xcode-command-line-tools/install/macos/tools-xcode-command-line-tools-install-macos.md)

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
$ which flutter
/opt/homebrew/bin/flutter
$ which dart
/opt/homebrew/bin/dart
```
