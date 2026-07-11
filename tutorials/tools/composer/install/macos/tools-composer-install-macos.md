[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [Composer](../../code-composer.md) > [Install](../tools-composer-install.md) > macOS

# Install Composer on macOS

This tutorial covers installing Composer on macOS systems.

## Prerequisites

- macOS 10.9 or higher
- PHP 7.0 or higher

## Installation Options

### Option 1: Install via Homebrew (Recommended)

```bash
brew install composer
```

### Option 2: Install via curl

```bash
curl -sS https://getcomposer.org/installer | php
mv composer.phar /usr/local/bin/composer
```

### Option 3: Install via installer

Download the Composer installer from https://getcomposer.org/ and run it:

```bash
php composer.phar install
```

## Verify Installation

Check that Composer is properly installed:

```bash
composer --version
```

## Troubleshooting

### Homebrew Installation Issues

If Homebrew fails to install:

```bash
brew uninstall composer
brew install composer
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
composer create-project --prefer-dist symfony/skeleton hello-world
```

## Additional Notes

Composer is a dependency manager for PHP. It's essential for managing PHP packages and dependencies in modern PHP projects.

### Security

Always verify your Composer installation:

```bash
composer verify
```

### Updates

To update Composer:

```bash
composer self-update
```

### Integration

Composer integrates well with modern PHP frameworks. It's a core component of PHP development.
