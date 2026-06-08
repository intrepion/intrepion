[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [Homebrew](../../tools-homebrew.md) > [Uninstall](../tools-homebrew-uninstall.md) > macOS

# Tools Homebrew Uninstall macOS

## Uninstall

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/uninstall.sh)"
```

## Remove Shell Configuration

Remove Homebrew paths from your shell configuration files.

```bash
vi ~/.zprofile
vi ~/.zshrc
vi ~/.bash_profile
```

Look for lines that mention Homebrew paths.

```text
/opt/homebrew/bin
/usr/local/bin
```

## Check Location

```bash
which -a brew
```

should print no paths

```text
$ which -a brew
```
