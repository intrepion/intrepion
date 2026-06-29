[Tutorials](../../../../tutorials.md) > [Code](../../../code.md) > [Dart](../../code-dart.md) > [Snippets](../code-dart-snippets.md) > .gitignore

# Code Dart Snippets .gitignore

## Add .gitignore file

```bash
touch .gitignore
printf '\n#### BEGIN https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Dart.gitignore\n\n' >> .gitignore
curl -sSL https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Dart.gitignore >> .gitignore
printf '\n#### END https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Dart.gitignore\n' >> .gitignore
git add .gitignore
git commit --message "Added Dart gitignores."
git push
```
