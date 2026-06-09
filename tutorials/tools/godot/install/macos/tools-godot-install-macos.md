[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [Godot](../../tools-godot.md) > [Install](../tools-godot-install.md) > macOS

# Tools Godot Install macOS

## Requirements

- [Homebrew](../../../homebrew/install/macos/tools-homebrew-install-macos.md)

## Install

```bash
brew install --cask godot
```

## Update

```bash
brew upgrade --cask godot
```

## Check Location

```bash
ls /Applications/Godot.app
```

should be something like

```text
$ ls /Applications/Godot.app
Contents
```

## Check Version

```bash
/Applications/Godot.app/Contents/MacOS/Godot --version
```

should be something like

```text
$ /Applications/Godot.app/Contents/MacOS/Godot --version
4.6.3.stable.official
```
