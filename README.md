cli-plugin-lighthouse
===================

vtex plugin template

[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
![npm](https://img.shields.io/npm/v/@vtex/cli-plugin-lighthouse)

<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g @vtex/cli-plugin-lighthouse
$ oclif-example COMMAND
running command...
$ oclif-example (-v|--version|version)
@vtex/cli-plugin-lighthouse/0.0.2 linux-x64 node-v12.18.3
$ oclif-example --help [COMMAND]
USAGE
  $ oclif-example COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`oclif-example lighthouse:audit URL`](#oclif-example-lighthouseaudit-url)
* [`oclif-example lighthouse:show`](#oclif-example-lighthouseshow)

## `oclif-example lighthouse:audit URL`

Run lighthouse audit over a specific url

```
USAGE
  $ oclif-example lighthouse:audit URL

OPTIONS
  -h, --help     show CLI help
  -j, --json     Return the report as json on stdout
  -v, --verbose  Show debug level logs
  --trace        Ensure all requests to VTEX IO are traced

ALIASES
  $ oclif-example lh:audit

EXAMPLES
  vtex lighthouse audit my.url.com
  vtex lh audit my.url.com
```

_See code: [build/commands/lighthouse/audit.ts](https://github.com/vtex/cli-plugin-lighthouse/blob/v0.0.2/build/commands/lighthouse/audit.ts)_

## `oclif-example lighthouse:show`

Show previous saved audit reports, filtering by app and/or url

```
USAGE
  $ oclif-example lighthouse:show

OPTIONS
  -a, --app=app  App name to be filtered
  -h, --help     show CLI help
  -u, --url=url  Url to be filtered
  -v, --verbose  Show debug level logs
  --trace        Ensure all requests to VTEX IO are traced

ALIASES
  $ oclif-example lh:show

EXAMPLES
  vtex lighthouse show --app=vtex.awesome-app
  vtex lighthouse show -u https://awesome.store.com
  vtex lighthouse show -a vtex.awesome-app --url=https://awesome.store.com
  vtex lh show --app=vtex.awesome-app
  vtex lh show -u https://awesome.store.com
  vtex lh show -a vtex.awesome-app --url=https://awesome.store.com
```

_See code: [build/commands/lighthouse/show.ts](https://github.com/vtex/cli-plugin-lighthouse/blob/v0.0.2/build/commands/lighthouse/show.ts)_
<!-- commandsstop -->
