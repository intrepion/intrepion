# Tools VSCodium Install macOS

## Requirements

- [Homebrew](../../../homebrew/install/macos/tools-homebrew-install-macos.md)

## Install

```bash
brew install --cask vscodium
```

## Update

```bash
brew upgrade --cask vscodium
```

## Install Shell Command

Open VSCodium and run `Shell Command: Install 'code' command in PATH` from the Command Palette.

## Check Location

```bash
which code
```

should be something like

```text
$ which code
/opt/homebrew/bin/code
```