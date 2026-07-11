[Tutorials](../../../../tutorials.md) > [Code](../../../code.md) > [.NET](../../code-dotnet.md) > [Snippets](../code-dotnet-snippets.md) > .gitignore

# Code .NET Snippets .gitignore

## Add .gitignore file

```bash
touch .gitignore
printf '\n#### BEGIN https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Dotnet.gitignore\n\n' >> .gitignore
curl -sSL https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Dotnet.gitignore >> .gitignore
printf '\n#### END https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Dotnet.gitignore\n' >> .gitignore
git add .gitignore
git commit --message "Added .NET gitignores."
git push
```
