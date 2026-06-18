[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [Hugging Face Hub](../../tools-huggingface-hub.md) > [Uninstall](../tools-huggingface-hub-uninstall.md) > macOS

# Tools Hugging Face Hub Uninstall macOS

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
