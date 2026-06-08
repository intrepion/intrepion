[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [Xcode Command Line Tools](../../tools-xcode-command-line-tools.md) > [Uninstall](../tools-xcode-command-line-tools-uninstall.md) > macOS

# Tools Xcode Command Line Tools Uninstall macOS

## Check Location

```bash
xcode-select --print-path
```

## Uninstall

```bash
sudo rm -rf /Library/Developer/CommandLineTools
```

## Reset Selected Developer Directory

```bash
sudo xcode-select --reset
```

## Check Location

```bash
xcode-select --print-path
```

should be something like

```text
$ xcode-select --print-path
xcode-select: error: unable to get active developer directory
```
