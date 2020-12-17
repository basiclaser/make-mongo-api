# api-make

[![oclif](https://img.shields.io/badge/lol-there%20are%20no%20tests-red.svg)](https://oclif.io)
[![Version](https://img.shields.io/npm/v/api-make.svg)](https://npmjs.org/package/api-make)
[![Downloads/week](https://img.shields.io/badge/-i%20have%20no%20idea%20what%20im%20doing-success)](https://npmjs.org/package/api-make)
[![License](https://img.shields.io/npm/l/api-make.svg)](https://github.com/basiclaser/api-make/blob/master/package.json)

initialise an api called "myProject":

`npx api-make init myProject`

go into the new project folder:

`cd myProject`

generate Message, Product and Review models, routes and controllers just like this!

`npx api-make add message product review`

add authentication register, login, logout, profile routes with password hashing and sessions, with a new User model.

`npx api-make auth user`

<!-- toc -->

- [api-make](#api-make)
- [quickstart](#quickstart)
- [Commands](#commands)
<!-- tocstop -->

# quickstart

<!-- usage -->

```sh-session
$ npm install -g api-make
$ api-make COMMAND
running command...
$ api-make (-v|--version|version)
api-make/1.0.3 darwin-x64 node-v12.19.0
$ api-make --help [COMMAND]
USAGE
  $ api-make COMMAND
...
```

<!-- usagestop -->

# Commands

<!-- commands -->

- [`api-make add [COLLECTION1] [COLLECTION2] [COLLECTION3] [COLLECTION4] [COLLECTION5]`](#api-make-add-collection1-collection2-collection3-collection4-collection5)
- [`api-make help [COMMAND]`](#api-make-help-command)
- [`api-make init [PROJECTNAME] [COLLECTION1] [COLLECTION2] [COLLECTION3] [COLLECTION4] [COLLECTION5]`](#api-make-init-projectname-collection1-collection2-collection3-collection4-collection5)

## `api-make add [COLLECTION1] [COLLECTION2] [COLLECTION3] [COLLECTION4] [COLLECTION5]`

generate new routes, controllers and a model by specifying a 'type'

```
USAGE
  $ api-make add [COLLECTION1] [COLLECTION2] [COLLECTION3] [COLLECTION4] [COLLECTION5]

DESCRIPTION
  eg. `api-make add event`

EXAMPLE
  $ api-make add message
  generates a Message model with routes and controllers
```

_See code: [src/commands/add.ts](https://github.com/basiclaser/api-make/blob/v1.0.3/src/commands/add.ts)_

## `api-make help [COMMAND]`

display help for api-make

```
USAGE
  $ api-make help [COMMAND]

ARGUMENTS
  COMMAND  command to show help for

OPTIONS
  --all  see all commands in CLI
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v3.2.1/src/commands/help.ts)_

## `api-make init [PROJECTNAME] [COLLECTION1] [COLLECTION2] [COLLECTION3] [COLLECTION4] [COLLECTION5]`

generates a blank api-make project

```
USAGE
  $ api-make init [PROJECTNAME] [COLLECTION1] [COLLECTION2] [COLLECTION3] [COLLECTION4] [COLLECTION5]

OPTIONS
  -f, --force
  -h, --help       show CLI help
  -n, --name=name  name to print

EXAMPLE
  $ api-make init <PROJECTNAME>
  generates a project folder called <PROJECTNAME>
```

_See code: [src/commands/init.ts](https://github.com/basiclaser/api-make/blob/v1.0.3/src/commands/init.ts)_

<!-- commandsstop -->

TODO: auth
`api-make --auth`
generates basic auth solution, user models, /register, /login, /logout, /profile routes and controllers

generate
/register
/login
/logout
/profile

TODO: postgreSQL
TODO: generate from a RAML/YAML file
TODO: loads of other things i'll never do
