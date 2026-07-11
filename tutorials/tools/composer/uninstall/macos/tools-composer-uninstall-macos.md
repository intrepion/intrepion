[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [Composer](../../code-composer.md) > [Uninstall](../tools-composer-uninstall.md) > macOS

# Uninstall Composer on macOS

This tutorial covers uninstalling Composer on macOS systems.

## Prerequisites

- Composer is installed on the system
- macOS 10.9 or higher

## Uninstall Options

### Option 1: Remove via Homebrew

```bash
brew uninstall composer
```

### Option 2: Remove manually

```bash
cd /usr/local/bin
rm composer
rm composer.phar
```

### Option 3: Complete removal

```bash
cd /usr/local/bin
rm -f composer*
```

## Verify Uninstall

Check that Composer is properly uninstalled:

```bash
which composer
```

## Troubleshooting

### Homebrew Removal Issues

If Homebrew fails to uninstall:

```bash
echo "Uninstalling via Homebrew failed"
```

### Manual Removal Issues

If manual removal fails:

```bash
cd /usr/local/bin
ls -la
```

## Configuration

### Path Configuration

Verify that Composer is removed from your shell profile:

```bash
cat ~/.bashrc | grep -i composer
```

### PHP Configuration

Verify PHP is still working:

```bash
php -v
```

## Additional Notes

Composer uninstallation removes only the composer binary. Any existing composer installations within projects will remain untouched.

### Security

Verify that no composer binaries remain:

```bash
find /usr -name "composer*" 2>/dev/null
```

### Integration

Composer uninstallation is typically only needed when switching to alternative dependency managers.

### Backup

Before uninstalling, you may want to backup your installed packages:

```bash
cp ~/.composer "backup/composer"
```
