[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [nvm](../../tools-nvm.md) > [Uninstall](../tools-nvm-uninstall.md) > macOS

# Tools nvm Uninstall macOS

## Remove nvm

```bash
rm -rf ~/.nvm
```

## Remove Shell Configuration

Remove nvm lines from your shell configuration files.

```bash
vi ~/.zshrc
vi ~/.bashrc
vi ~/.bash_profile
```

Look for lines like these.

```bash
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"
```

## Check Location

```bash
ls ~/.nvm/nvm.sh
which -a node
which -a npm
```

should print no nvm path

```text
$ ls ~/.nvm/nvm.sh
ls: /Users/oliverforral/.nvm/nvm.sh: No such file or directory
$ which -a node
$ which -a npm
```

If Node.js is installed another way, `node` and `npm` may still print paths.
