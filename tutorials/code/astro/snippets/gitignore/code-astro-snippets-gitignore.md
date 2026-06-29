[Tutorials](../../../../tutorials.md) > [Code](../../../code.md) > [Astro](../../code-astro.md) > [Snippets](../code-astro-snippets.md) > .gitignore

# Code Astro Snippets .gitignore

## Add .gitignore file

```bash
touch .gitignore
printf '%s\n' \
  '' \
  '#### BEGIN Astro' \
  '' \
  '# generated types' \
  '.astro/' \
  '' \
  '#### END Astro' \
  | tee -a .gitignore > /dev/null
git add .gitignore
git commit --message "Added Astro gitignores."
git push
```
