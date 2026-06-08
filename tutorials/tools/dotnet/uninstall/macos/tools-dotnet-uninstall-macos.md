[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [.NET](../../tools-dotnet.md) > [Uninstall](../tools-dotnet-uninstall.md) > macOS

# Tools .NET Uninstall macOS

## Uninstall

```bash
brew uninstall --cask dotnet-sdk
```

## Remove Installed SDKs and Runtimes

```bash
sudo rm -rf /usr/local/share/dotnet
sudo rm -f /usr/local/bin/dotnet
sudo rm -f /etc/paths.d/dotnet
```

## Check Location

```bash
which -a dotnet
```

should print no paths

```text
$ which -a dotnet
```
