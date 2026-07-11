# Composer Snippets

This section contains code snippets for Composer development.

- [.gitignore](./snippets/gitignore/code-composer-snippets-gitignore.md)

## Overview

Code snippets for Composer development help accelerate your workflow. This section provides useful code samples that can be directly copied and used in your PHP projects.

## Available Snippets

### .gitignore

The .gitignore snippet contains the necessary entries to exclude build artifacts and temporary files from version control. Use the [gitignore](./snippets/gitignore/code-composer-snippets-gitignore.md) snippet to quickly add PHP-specific gitignore rules to your repository.

### composer.json

The composer.json snippet contains a basic configuration template for your PHP project. Use this to initialize your project with appropriate dependencies.

### Installation

To use this snippet:

```bash
composer init
```

### Dependencies

To add a dependency:

```bash
composer require vendor/package
```

### Update

To update dependencies:

```bash
composer update
```

### Autoloading

To generate autoloading files:

```bash
composer dump-autoload
```

### Installation

To install dependencies:

```bash
composer install
```

### Versioning

To update version:

```bash
composer require --dev vendor/package
```

### Development

To run development:

```bash
php -S localhost:8000
```

### Testing

To run tests:

```bash
vendor/bin/phpunit
```

### Documentation

To generate documentation:

```bash
phpdoc
```

### Configuration

To configure Composer:

```bash
composer config --global repositories.packagist https://packagist.org
```

### Troubleshooting

To clear cache:

```bash
composer clear-cache
```

### Environment

To set environment variables:

```bash
export COMPOSER_CACHE_DIR=/tmp/composer_cache
```
