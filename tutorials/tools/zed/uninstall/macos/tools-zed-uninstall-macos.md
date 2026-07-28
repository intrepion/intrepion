[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [Zed](../../tools-zed.md) > [Uninstall](../tools-zed-uninstall.md) > macOS

# Tools Zed Uninstall macOS

## Uninstall

```bash
brew uninstall --cask zed
```

## Remove User Data

```bash
rm -rf ~/.config/zed
rm -rf ~/Library/Application\ Support/Zed
rm -rf ~/Library/Caches/dev.zed.Zed
```

## Check Location

```bash
which -a zed
ls /Applications/Zed.app
```

should be something like

```text
$ which -a zed
$ ls /Applications/Zed.app
ls: /Applications/Zed.app: No such file or directory
```
