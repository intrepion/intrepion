[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [Visual Studio Code](../../tools-visual-studio-code.md) > [Uninstall](../tools-visual-studio-code-uninstall.md) > macOS

# Tools Visual Studio Code Uninstall macOS

## Uninstall

```bash
brew uninstall --cask visual-studio-code
```

## Remove User Data

```bash
rm -rf ~/Library/Application\ Support/Code
rm -rf ~/Library/Caches/com.microsoft.VSCode
rm -rf ~/Library/Preferences/com.microsoft.VSCode.plist
rm -rf ~/.vscode
```

## Check Location

```bash
which -a code
ls /Applications/Visual\ Studio\ Code.app
```

should be something like

```text
$ which -a code
$ ls /Applications/Visual\ Studio\ Code.app
ls: /Applications/Visual Studio Code.app: No such file or directory
```
