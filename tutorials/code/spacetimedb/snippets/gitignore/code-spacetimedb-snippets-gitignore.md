[Tutorials](../../../../tutorials.md) > [Code](../../../code.md) > [SpaceTimeDB](../../code-spacetimedb.md) > [Snippets](../code-spacetimedb-snippets.md) > .gitignore

# Code SpaceTimeDB Snippets .gitignore

## Add .gitignore file

```bash
touch .gitignore
printf '%s\n' \
  '' \
  '#### BEGIN SpaceTimeDB' \
  '' \
  '# generated client bindings' \
  'src/module_bindings/' \
  '' \
  '#### END SpaceTimeDB' \
  | tee -a .gitignore > /dev/null
```
