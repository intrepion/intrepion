[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [Bash](../../tools-bash.md) > [Uninstall](../tools-bash-uninstall.md) > macOS

# Tools Bash Uninstall macOS

## Check Current Shell

```bash
echo "$SHELL"
```

If your shell is the Homebrew Bash path, change it before uninstalling.

```bash
chsh -s /bin/bash
```

## Uninstall

```bash
brew uninstall bash
```

## Remove Shell Entry

```bash
sudo vi /etc/shells
```

Remove this line if it exists.

```text
/opt/homebrew/bin/bash
```

## Check Location

```bash
which -a bash
```

should be something like

```text
$ which -a bash
/bin/bash
```
