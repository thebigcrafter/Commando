# Commando

Commando is a command framework virion for PocketMine-MP API 5. This repository is the thebigcrafter fork of the modified Commando distribution maintained by Paroxity, published independently because the modified package was not available on Packagist under the required coordinates.

## Installation

Install the Composer package for development or consumer integration:

```sh
composer require thebigcrafter/commando
```

For a PocketMine-MP plugin, include the virion in the plugin's packaging workflow and use the `CortexPE\\Commando` namespace. The `virion.yml` manifest is the source of truth for the embedded virion metadata.

## Compatibility

- PHP 8.1 or newer
- PocketMine-MP API 5; the current manifest baseline is API 5.36.0
- Virion specification 3.1

This is a library/virion, not a standalone PocketMine-MP plugin. Build and runtime validation must be performed through a compatible plugin consumer.

## Development checks

Install the locked development dependencies and run the maximum-level PHPStan configuration:

```sh
composer install
composer analyze
```

The repository does not define a standalone plugin PHAR workflow. Consumer packaging should use the DevTools policy of the consuming plugin.

## Attribution and license

Commando is derived from [CortexPE/Commando](https://github.com/CortexPE/Commando) and incorporates modifications from [Paroxity/Commando](https://github.com/Paroxity/Commando). Preserve the upstream notices and the repository's LGPL-3.0-only license when redistributing it.
