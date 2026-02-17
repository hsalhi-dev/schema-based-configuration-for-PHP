# League Config

A flexible PHP configuration management library.

## Overview

League Config provides a structured way to manage application configuration in PHP. It offers:

- **Type-safe configuration** with validation
- **Dotted key access** for nested configuration values
- **Schema-driven configuration** building
- **Immutable configuration** objects for read-only access

## Installation

```bash
composer require league/config
```

## Quick Start

```php
use League\Config\ConfigurationBuilder;

$builder = new ConfigurationBuilder();
// Configure your schema and build configuration
$config = $builder->build();

// Access configuration values
$value = $config->get('path.to.key');
```

## Development

This project uses the following tools for code quality:

- **PHP CodeSniffer (PHPCS)** - Detects violations of PHP coding standards
- **PHPStan** - Static analysis tool for finding bugs and type errors

Running code quality checks:

```bash
# Run PHPCS
./vendor/bin/phpcs

# Fix PHPCS issues
./vendor/bin/phpcbf

# Run PHPStan
./vendor/bin/phpstan
```

## Requirements

- PHP 7.4 or higher
- `dflydev/dot-access-data` for nested array access
- `nette/schema` for configuration schema validation

## License

This package is licensed under the MIT License. See the LICENSE file for details.
