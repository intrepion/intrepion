[Tutorials](../../../../tutorials.md) > [Code](../../../code.md) > [Unity](../../code-unity.md) > [Snippets](../code-unity-snippets.md) > .gitignore

# Code Unity Snippets .gitignore

## Add .gitignore file

```bash
touch .gitignore
printf '\n#### BEGIN https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Unity.gitignore\n\n' >> .gitignore
curl -sSL https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Unity.gitignore >> .gitignore
printf '\n#### END https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Unity.gitignore\n' >> .gitignore
git add .gitignore
git commit --message "Added Unity gitignores."
git push
```
