[Tutorials](../../../tutorials.md) > [Code](../../code.md) > [Common](../code-common.md) > .gitignore

# Code Common .gitignore

## Add .gitignore file

```bash
touch .gitignore
printf '#### BEGIN https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Global/Linux.gitignore\n\n' >> .gitignore
curl -sSL https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Global/Linux.gitignore >> .gitignore
printf '\n#### END https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Global/Linux.gitignore\n' >> .gitignore
printf '\n#### BEGIN https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Global/Windows.gitignore\n\n' >> .gitignore
curl -sSL https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Global/Windows.gitignore >> .gitignore
printf '\n#### END https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Global/Windows.gitignore\n' >> .gitignore
printf '\n#### BEGIN https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Global/macOS.gitignore\n\n' >> .gitignore
curl -sSL https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Global/macOS.gitignore >> .gitignore
printf '\n#### END https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Global/macOS.gitignore\n' >> .gitignore
git add .gitignore
git commit --message "Added operating system gitignores."
git push
```
