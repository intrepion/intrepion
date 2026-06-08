[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [CocoaPods](../../tools-cocoapods.md) > [Uninstall](../tools-cocoapods-uninstall.md) > macOS

# Tools CocoaPods Uninstall macOS

## Uninstall

```bash
brew uninstall cocoapods
```

## Remove User Cache

```bash
rm -rf ~/.cocoapods
rm -rf ~/Library/Caches/CocoaPods
```

## Check Location

```bash
which -a pod
```

should print no paths

```text
$ which -a pod
```
