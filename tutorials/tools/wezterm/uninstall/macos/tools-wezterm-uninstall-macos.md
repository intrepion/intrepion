[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [WezTerm](../../tools-wezterm.md) > [Uninstall](../tools-wezterm-uninstall.md) > macOS

# Tools WezTerm Uninstall macOS

## Uninstall

```bash
brew uninstall --cask wezterm
```

## Remove User Data

```bash
rm -rf ~/.local/share/wezterm
rm -rf ~/Library/Application\ Support/wezterm
rm -rf ~/Library/Caches/wezterm
```

## Check Location

```bash
which -a wezterm
```

should print no paths

```text
$ which -a wezterm
```
