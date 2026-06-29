[Tutorials](../../../../tutorials.md) > [Code](../../../code.md) > [SpaceTimeDB](../../code-spacetimedb.md) > [Snippets](../code-spacetimedb-snippets.md) > .gitignore

# Code SpaceTimeDB Snippets .gitignore

## Add .gitignore file

```bash
touch .gitignore
printf '%s\n' \
  '' \
  '#### BEGIN SpacetimeDB' \
  '' \
  '# generated client bindings' \
  'src/module_bindings/' \
  '' \
  '#### END SpacetimeDB' \
  | tee -a .gitignore > /dev/null
git add .gitignore
git commit --message "Added SpacetimeDB gitignores"
git push
```
