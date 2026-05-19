[Tutorials](../../../../tutorials.md) > [Homebrew](../../homebrew.md) > [Homebrew Install](../homebrew-install.md) > Homebrew Install macOS

# Homebrew Install macOS

## Install

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## Update all package definitions (formulae) and Homebrew itself

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
/opt/homebrew/bin/brew
```
