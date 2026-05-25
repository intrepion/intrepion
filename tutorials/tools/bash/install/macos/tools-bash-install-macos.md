[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [Bash](../../tools-bash.md) > [Install](../tools-bash-install.md) > macOS

# Tools Bash Install macOS

## Requirements

- [Homebrew](../../../homebrew/install/macos/tools-homebrew-install-macos.md)

## Install

```bash
echo $SHELL
echo $BASH_VERSION
brew install bash
/opt/homebrew/bin/bash --version
sudo vi /etc/shells
```

```text
/opt/homebrew/bin/bash
```

```text
<Esc>:x
```

```bash
chsh -s /opt/homebrew/bin/bash
echo $SHELL
echo $BASH_VERSION
```

## Check Location

```bash
which bash
```

should be something like

```text
/opt/homebrew/bin/bash
```
