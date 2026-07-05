# Tools VSCodium Uninstall

## Uninstall

```bash
brew uninstall --cask vscodium
```

## Remove Configuration

```bash
rm -rf ~/.config/vscodium
```

## Remove Cache

```bash
rm -rf ~/.cache/vscodium
```

## Remove Logs

```bash
rm -rf ~/.local/share/vscodium
```

## Verify Removal

```bash
which code
```

should return nothing or an error.

## Notes

VSCodium is installed as a Cask through Homebrew. To completely remove all related files:

1. Remove the application using Homebrew
2. Remove any configuration files
3. Remove any cache files

VSCodium stores its configuration files under `~/.config/vscodium`.

VSCodium is a free and open-source alternative to Visual Studio Code that removes Microsoft's telemetry and branding.