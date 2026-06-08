[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [Neovim](../../tools-neovim.md) > [Uninstall](../tools-neovim-uninstall.md) > macOS

# Tools Neovim Uninstall macOS

## Uninstall

```bash
brew uninstall neovim
```

## Remove User Data

```bash
rm -rf ~/.local/share/nvim
rm -rf ~/.local/state/nvim
rm -rf ~/.cache/nvim
```

## Check Location

```bash
which -a nvim
```

should print no paths

```text
$ which -a nvim
```
