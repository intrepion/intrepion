[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [SpacetimeDB](../../tools-spacetimedb.md) > [Uninstall](../tools-spacetimedb-uninstall.md) > macOS

# Tools SpacetimeDB Uninstall macOS

## Remove Binary

```bash
rm -f ~/.local/bin/spacetime
```

## Remove User Data

```bash
rm -rf ~/.spacetime
rm -rf ~/.config/spacetime
```

## Check Location

```bash
which -a spacetime
```

should print no paths

```text
$ which -a spacetime
```
