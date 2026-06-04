[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [Android Studio](../../tools-android-studio.md) > [Install](../tools-android-studio-install.md) > macOS

# Tools Android Studio Install macOS

## Requirements

- [Homebrew](../../../homebrew/install/macos/tools-homebrew-install-macos.md)

## Install

```bash
brew install --cask android-studio
```

## Update

```bash
brew upgrade --cask android-studio
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

## Check Location

```bash
ls /Applications/Android\ Studio.app
```
