[Tutorials](../../../../tutorials.md) > [Code](../../../code.md) > [Go](../../code-go.md) > [Snippets](../code-go-snippets.md) > .gitignore

# Code Go Snippets .gitignore

## Add .gitignore file

```bash
touch .gitignore
printf '\n#### BEGIN https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Go.gitignore\n\n' >> .gitignore
curl -sSL https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Go.gitignore >> .gitignore
printf '\n#### END https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Go.gitignore\n' >> .gitignore
git add .gitignore
git commit --message "Added Go gitignores."
git push
```
