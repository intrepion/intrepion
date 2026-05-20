[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [Visual Studio Code](../../visual-studio-code.md) > [Visual Studio Code Install](../visual-studio-code-install.md) > Visual Studio Code Install macOS

# Visual Studio Code Install macOS

## Requirements

- [Homebrew](../../../homebrew/install/macos/homebrew-install-macos.md)

## Install

```bash
brew install --cask visual-studio-code
```

## Install Shell Command

Open Visual Studio Code and run `Shell Command: Install 'code' command in PATH` from the Command Palette.

## Check Location

```bash
which code
ls /Applications/Visual\ Studio\ Code.app
```

should be something like

```text
$ which code
/opt/homebrew/bin/code
$ ls /Applications/Visual\ Studio\ Code.app
Contents
```
