[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [PHP](../../code-php.md) > [Uninstall](../tools-php-uninstall.md) > macOS

# Uninstall PHP on macOS

This tutorial covers uninstalling PHP on macOS systems.

## Prerequisites

- PHP is installed on the system
- macOS 10.9 or higher

## Uninstall Options

### Option 1: Remove via Homebrew

```bash
brew uninstall php
```

### Option 2: Remove manually

```bash
cd /usr/local/bin
rm php
rm php-config
rm php-fpm
```

### Option 3: Complete removal

```bash
cd /usr/local/bin
rm -f php*
```

## Verify Uninstall

Check that PHP is properly uninstalled:

```bash
which php
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

Verify that PHP is removed from your shell profile:

```bash
cat ~/.bashrc | grep -i php
```

### PHP Configuration

Verify PHP is no longer installed:

```bash
php --version
```

## Additional Notes

PHP uninstallation removes only the php binaries. Any existing php installations within projects will remain untouched.

### Security

Verify that no php binaries remain:

```bash
find /usr -name "php*" 2>/dev/null
```

### Integration

PHP uninstallation is typically only needed when switching to alternative PHP versions.

### Backup

Before uninstalling, you may want to backup your installed packages:

```bash
cp ~/.php "backup/php"
```
