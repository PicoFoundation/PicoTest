## Description

The `wallet_plugin` adds access to wallet functionality from a node.

[[caution | Caution]]
| This plugin is not designed to be loaded as a plugin on a publicly accessible node without further security measures. This is particularly true when loading the `wallet_api_plugin`, which should not be loaded on a publicly accessible node under any circumstances.

## Usage

```sh
# config.ini
plugin = picoio::wallet_plugin

# command-line
nodpico ... --plugin picoio::wallet_plugin
```

## Options

None

## Dependencies

* [`wallet_plugin`](../wallet_plugin/index.md)
* [`http_plugin`](../http_plugin/index.md)

### Load Dependency Examples

```sh
# config.ini
plugin = picoio::wallet_plugin
[options]
plugin = picoio::http_plugin
[options]

# command-line
nodpico ... --plugin picoio::wallet_plugin [options]  \
           --plugin picoio::http_plugin [options]
```
