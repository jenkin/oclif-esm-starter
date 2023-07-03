oclif-hello-world
=================

oclif example Hello World CLI

[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![CircleCI](https://circleci.com/gh/oclif/hello-world/tree/main.svg?style=shield)](https://circleci.com/gh/oclif/hello-world/tree/main)
[![GitHub license](https://img.shields.io/github/license/oclif/hello-world)](https://github.com/oclif/hello-world/blob/main/LICENSE)

<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g oclif-esm-starter
$ oclif-esm-starter COMMAND
running command...
$ oclif-esm-starter (--version)
oclif-esm-starter/0.0.0 linux-x64 node-v18.16.0
$ oclif-esm-starter --help [COMMAND]
USAGE
  $ oclif-esm-starter COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`oclif-esm-starter hello PERSON`](#oclif-esm-starter-hello-person)
* [`oclif-esm-starter hello world`](#oclif-esm-starter-hello-world)
* [`oclif-esm-starter help [COMMANDS]`](#oclif-esm-starter-help-commands)
* [`oclif-esm-starter plugins`](#oclif-esm-starter-plugins)
* [`oclif-esm-starter plugins:install PLUGIN...`](#oclif-esm-starter-pluginsinstall-plugin)
* [`oclif-esm-starter plugins:inspect PLUGIN...`](#oclif-esm-starter-pluginsinspect-plugin)
* [`oclif-esm-starter plugins:install PLUGIN...`](#oclif-esm-starter-pluginsinstall-plugin-1)
* [`oclif-esm-starter plugins:link PLUGIN`](#oclif-esm-starter-pluginslink-plugin)
* [`oclif-esm-starter plugins:uninstall PLUGIN...`](#oclif-esm-starter-pluginsuninstall-plugin)
* [`oclif-esm-starter plugins:uninstall PLUGIN...`](#oclif-esm-starter-pluginsuninstall-plugin-1)
* [`oclif-esm-starter plugins:uninstall PLUGIN...`](#oclif-esm-starter-pluginsuninstall-plugin-2)
* [`oclif-esm-starter plugins update`](#oclif-esm-starter-plugins-update)

## `oclif-esm-starter hello PERSON`

Say hello

```
USAGE
  $ oclif-esm-starter hello PERSON -f <value>

ARGUMENTS
  PERSON  Person to say hello to

FLAGS
  -f, --from=<value>  (required) Who is saying hello

DESCRIPTION
  Say hello

EXAMPLES
  $ oex hello friend --from oclif
  hello friend from oclif! (./src/commands/hello/index.ts)
```

_See code: [dist/commands/hello/index.ts](https://github.com/jenkin/oclif-esm-starter/blob/v0.0.0/dist/commands/hello/index.ts)_

## `oclif-esm-starter hello world`

Say hello world

```
USAGE
  $ oclif-esm-starter hello world

DESCRIPTION
  Say hello world

EXAMPLES
  $ oclif-esm-starter hello world
  hello world! (./src/commands/hello/world.ts)
```

## `oclif-esm-starter help [COMMANDS]`

Display help for oclif-esm-starter.

```
USAGE
  $ oclif-esm-starter help [COMMANDS] [-n]

ARGUMENTS
  COMMANDS  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for oclif-esm-starter.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v5.2.10/src/commands/help.ts)_

## `oclif-esm-starter plugins`

List installed plugins.

```
USAGE
  $ oclif-esm-starter plugins [--core]

FLAGS
  --core  Show core plugins.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ oclif-esm-starter plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v2.4.7/src/commands/plugins/index.ts)_

## `oclif-esm-starter plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ oclif-esm-starter plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.
  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.


ALIASES
  $ oclif-esm-starter plugins add

EXAMPLES
  $ oclif-esm-starter plugins:install myplugin 

  $ oclif-esm-starter plugins:install https://github.com/someuser/someplugin

  $ oclif-esm-starter plugins:install someuser/someplugin
```

## `oclif-esm-starter plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ oclif-esm-starter plugins:inspect PLUGIN...

ARGUMENTS
  PLUGIN  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ oclif-esm-starter plugins:inspect myplugin
```

## `oclif-esm-starter plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ oclif-esm-starter plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.
  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.


ALIASES
  $ oclif-esm-starter plugins add

EXAMPLES
  $ oclif-esm-starter plugins:install myplugin 

  $ oclif-esm-starter plugins:install https://github.com/someuser/someplugin

  $ oclif-esm-starter plugins:install someuser/someplugin
```

## `oclif-esm-starter plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ oclif-esm-starter plugins:link PLUGIN

ARGUMENTS
  PATH  [default: .] path to plugin

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Links a plugin into the CLI for development.
  Installation of a linked plugin will override a user-installed or core plugin.

  e.g. If you have a user-installed or core plugin that has a 'hello' command, installing a linked plugin with a 'hello'
  command will override the user-installed or core plugin implementation. This is useful for development work.


EXAMPLES
  $ oclif-esm-starter plugins:link myplugin
```

## `oclif-esm-starter plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ oclif-esm-starter plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ oclif-esm-starter plugins unlink
  $ oclif-esm-starter plugins remove
```

## `oclif-esm-starter plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ oclif-esm-starter plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ oclif-esm-starter plugins unlink
  $ oclif-esm-starter plugins remove
```

## `oclif-esm-starter plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ oclif-esm-starter plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ oclif-esm-starter plugins unlink
  $ oclif-esm-starter plugins remove
```

## `oclif-esm-starter plugins update`

Update installed plugins.

```
USAGE
  $ oclif-esm-starter plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```
<!-- commandsstop -->
