[Tutorials](../../../../tutorials.md) > [Code](../../../code.md) > [Rust](../../code-rust.md) > [Snippets](../code-rust-snippets.md) > .gitignore

# Code Rust Snippets .gitignore

## Add .gitignore file

```bash
touch .gitignore
printf '\n#### BEGIN https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Rust.gitignore\n\n' >> .gitignore
curl -sSL https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Rust.gitignore >> .gitignore
printf '\n#### END https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Rust.gitignore\n' >> .gitignore
```
