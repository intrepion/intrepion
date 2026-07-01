[Tutorials](../../../../tutorials.md) > [Code](../../../code.md) > [C#](../../code-csharp.md) > [Snippets](../code-csharp-snippets.md) > .gitignore

# Code C# Snippets .gitignore

## Add .gitignore file

```bash
touch .gitignore
printf '\n#### BEGIN https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Dotnet.gitignore\n\n' >> .gitignore
curl -sSL https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Dotnet.gitignore >> .gitignore
printf '\n#### END https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Dotnet.gitignore\n' >> .gitignore
git add .gitignore
git commit --message "Added C# gitignores."
git push
```
