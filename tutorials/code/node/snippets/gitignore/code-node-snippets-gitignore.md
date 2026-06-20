[Tutorials](../../../../tutorials.md) > [Code](../../../code.md) > [Node](../../code-node.md) > [Snippets](../code-node-snippets.md) > .gitignore

# Code Node Snippets .gitignore

## Add .gitignore file

```bash
touch .gitignore
printf '\n#### BEGIN https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Node.gitignore\n\n' >> .gitignore
curl -sSL https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Node.gitignore >> .gitignore
printf '\n#### END https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Node.gitignore\n' >> .gitignore
```
