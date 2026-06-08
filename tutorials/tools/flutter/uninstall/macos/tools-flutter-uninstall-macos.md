[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [Flutter](../../tools-flutter.md) > [Uninstall](../tools-flutter-uninstall.md) > macOS

# Tools Flutter Uninstall macOS

## Uninstall

```bash
brew uninstall --cask flutter
```

## Remove User Data

```bash
rm -rf ~/.flutter
rm -rf ~/.dart
rm -rf ~/.pub-cache
rm -rf ~/Library/Application\ Support/io.flutter
```

## Check Location

```bash
which -a flutter
which -a dart
```

should print no paths

```text
$ which -a flutter
$ which -a dart
```
