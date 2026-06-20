[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [HF CLI](../../tools-hf-cli.md) > [Uninstall](../tools-hf-cli-uninstall.md) > macOS

# Tools HF CLI Uninstall macOS

## Uninstall

```bash
hf auth logout
rm -f ~/.local/bin/hf
```

## Remove User Data

```bash
rm -rf ~/.cache/huggingface
```

## Check Location

```bash
which -a hf
```

should print no paths

```text
$ which -a hf
```
