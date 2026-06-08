[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [Unity Hub](../../tools-unity-hub.md) > [Uninstall](../tools-unity-hub-uninstall.md) > macOS

# Tools Unity Hub Uninstall macOS

## Uninstall

```bash
brew uninstall --cask unity-hub
```

## Remove User Data

```bash
rm -rf ~/Library/Application\ Support/UnityHub
rm -rf ~/Library/Caches/com.unity3d.unityhub
rm -rf ~/Library/Preferences/com.unity3d.unityhub.plist
```

## Check Location

```bash
ls /Applications/Unity\ Hub.app
```

should be something like

```text
$ ls /Applications/Unity\ Hub.app
ls: /Applications/Unity Hub.app: No such file or directory
```
