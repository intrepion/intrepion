[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [Xcode Command Line Tools](../../tools-xcode-command-line-tools.md) > [Install](../tools-xcode-command-line-tools-install.md) > macOS

# Tools Xcode Command Line Tools Install macOS

## Install

```bash
xcode-select --install
```

## Update

Open `System Settings > General > Software Update` and install available Command Line Tools updates.

## Check Location

```bash
xcode-select --print-path
```

should be something like

```text
$ xcode-select --print-path
/Applications/Xcode.app/Contents/Developer
```
