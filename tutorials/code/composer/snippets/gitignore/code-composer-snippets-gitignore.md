[Tutorials](../../../../tutorials.md) > [Code](../../../code.md) > [Composer](../../code-composer.md) > [Snippets](../code-composer-snippets.md) > .gitignore

# Code Composer Snippets .gitignore

## Add .gitignore file

```bash
.touch .gitignore
printf '\n#### BEGIN https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Composer.gitignore\n\n' >> .gitignore
curl -sSL https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Composer.gitignore >> .gitignore
printf '\n#### END https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Composer.gitignore\n' >> .gitignore
git add .gitignore
git commit --message "Added Composer gitignores."
git push
```
