[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [Homebrew](../../tools-homebrew.md) > [Install](../tools-homebrew-install.md) > macOS

# Tools Homebrew Install macOS

## Install

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## Update

```bash
brew update
```

## List which of your installed packages (kegs) are outdated

```bash
brew outdated
```

## Upgrade everything

```bash
brew upgrade
```

## Check Location

```bash
which brew
```

should be something like

```text
$ which brew
/opt/homebrew/bin/brew
```
