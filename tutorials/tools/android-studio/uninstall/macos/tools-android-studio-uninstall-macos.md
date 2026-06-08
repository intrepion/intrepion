[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [Android Studio](../../tools-android-studio.md) > [Uninstall](../tools-android-studio-uninstall.md) > macOS

# Tools Android Studio Uninstall macOS

## Uninstall

```bash
brew uninstall --cask android-studio
```

## Remove User Data

```bash
rm -rf ~/Library/Application\ Support/Google/AndroidStudio*
rm -rf ~/Library/Caches/Google/AndroidStudio*
rm -rf ~/Library/Logs/Google/AndroidStudio*
rm -rf ~/Library/Preferences/Google/AndroidStudio*
```

## Remove Android SDK

```bash
rm -rf ~/Library/Android/sdk
```

## Check Location

```bash
ls /Applications/Android\ Studio.app
```

should be something like

```text
$ ls /Applications/Android\ Studio.app
ls: /Applications/Android Studio.app: No such file or directory
```
