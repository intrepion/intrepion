[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [Godot](../../tools-godot.md) > [Uninstall](../tools-godot-uninstall.md) > macOS

# Tools Godot Uninstall macOS

## Uninstall

```bash
brew uninstall --cask godot
```

## Remove User Data

```bash
rm -rf ~/Library/Application\ Support/Godot
rm -rf ~/Library/Caches/Godot
rm -rf ~/Library/Preferences/org.godotengine.godot.plist
rm -rf ~/Library/Saved\ Application\ State/org.godotengine.godot.savedState
```

## Check Location

```bash
ls /Applications/Godot.app
```

should be something like

```text
$ ls /Applications/Godot.app
ls: /Applications/Godot.app: No such file or directory
```
