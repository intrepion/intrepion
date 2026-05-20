[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [Android Studio](../../android-studio.md) > [Android Studio Install](../android-studio-install.md) > Android Studio Install macOS

# Android Studio Install macOS

## Requirements

- [Homebrew](../../../homebrew/install/macos/homebrew-install-macos.md)

## Install

```bash
brew install --cask android-studio
```

## Setup

Open Android Studio and complete the Setup Wizard.

## Install Android SDK Components

Open Android Studio and go to `Tools > SDK Manager`.

If the Welcome screen is open, go to `More Actions > SDK Manager`.

In `SDK Platforms`, install:

- Android SDK Platform, API 36 or newer

In `SDK Tools`, install:

- Android SDK Build-Tools
- Android SDK Command-line Tools (latest)
- Android Emulator
- Android SDK Platform-Tools

If `Android SDK Command-line Tools (latest)` is not visible, check `Show Package Details`.

Click `Apply` to install the selected components.

The Android SDK location should be something like:

```text
/Users/oliverforral/Library/Android/sdk
```

## Check Android SDK Location

```bash
ls ~/Library/Android/sdk
```

should include something like

```text
$ ls ~/Library/Android/sdk
build-tools
cmdline-tools
emulator
licenses
platform-tools
platforms
sources
```

## Check Android SDK Command Line Tools

```bash
ls ~/Library/Android/sdk/cmdline-tools/latest/bin/sdkmanager
```

should be something like

```text
$ ls ~/Library/Android/sdk/cmdline-tools/latest/bin/sdkmanager
/Users/oliverforral/Library/Android/sdk/cmdline-tools/latest/bin/sdkmanager
```

## Check Version

```bash
studio --version
```

should be something like

```text
$ studio --version
Android Studio Panda 4 | 2025.3.4 Patch 1
Build #AI-253.32098.37.2534.15336583
```

## Check Location

```bash
ls /Applications/Android\ Studio.app
```
