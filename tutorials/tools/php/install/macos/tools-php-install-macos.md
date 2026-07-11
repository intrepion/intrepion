[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [PHP](../../code-php.md) > [Install](../tools-php-install.md) > macOS

# Install PHP on macOS

This tutorial covers installing PHP on macOS systems.

## Prerequisites

- macOS 10.9 or higher
- Xcode Command Line Tools

## Installation Options

### Option 1: Install via Homebrew (Recommended)

```bash
brew install php
```

### Option 2: Install via MacPorts

```bash
sudo port install php
```

### Option 3: Install via installer

Download the PHP installer from https://www.php.net/downloads.php and run it:

```bash
sudo installer -pkg php-8.1.0.pkg -target /
```

## Verify Installation

Check that PHP is properly installed:

```bash
php --version
```

## Troubleshooting

### Homebrew Installation Issues

If Homebrew fails to install:

```bash
brew uninstall php
brew install php
```

### Manual Installation Issues

If manual installation fails:

```bash
php -m
```

## Configuration

### Path Configuration

Add to your shell profile:

```bash
export PATH="$PATH:/usr/local/bin"
```

### PHP Configuration

Verify PHP installation:

```bash
php -v
```

### Test Installation

```bash
echo 'Hello World' > hello.php
php hello.php
```

## Additional Notes

PHP is a popular general-purpose scripting language that is especially suited for web development.

### Security

Always verify your PHP installation:

```bash
php -S localhost:8000
```

### Updates

To update PHP:

```bash
curl -O https://www.php.net/get/php-8.1.0.tar.gz
```

### Integration

PHP integrates well with web servers and databases. It's a core component of web development.
