---
title: npm-set-script
section: 1
description: Set tasks in the scripts section of package.json
redirect_from:
  - /cli/set-script
  - /cli/set-script.html
  - /cli/commands/set-script
  - /cli-commands/set-script
  - /cli-commands/set-script.html
  - /cli-commands/npm-set-script
github_repo: npm/cli
github_branch: latest
github_path: docs/content/commands/npm-set-script.md
---

### Synopsis
An npm command that lets you create a task in the `scripts` section of the `package.json`.

```bash
npm set-script [<script>] [<command>]
```


**Example:**

* `npm set-script start "http-server ."`

```json
{
  "name": "my-project",
  "scripts": {
    "start": "http-server .",
    "test": "some existing value"
  }
}
```

### Configuration

<!-- AUTOGENERATED CONFIG DESCRIPTIONS START -->
<!-- automatically generated, do not edit manually -->
<!-- see lib/utils/config/definitions.js -->
#### `workspace`

* Default:
* Type: String (can be set multiple times)

Enable running a command in the context of the configured workspaces of the
current project while filtering by running only the workspaces defined by
this configuration option.

Valid values for the `workspace` config are either:

* Workspace names
* Path to a workspace directory
* Path to a parent workspace directory (will result to selecting all of the
  nested workspaces)

When set for the `npm init` command, this may be set to the folder of a
workspace which does not yet exist, to create the folder and set it up as a
brand new workspace within the project.

This value is not exported to the environment for child processes.

<!-- automatically generated, do not edit manually -->
<!-- see lib/utils/config/definitions.js -->

#### `workspaces`

* Default: false
* Type: Boolean

Enable running a command in the context of **all** the configured
workspaces.

This value is not exported to the environment for child processes.

<!-- automatically generated, do not edit manually -->
<!-- see lib/utils/config/definitions.js -->

<!-- AUTOGENERATED CONFIG DESCRIPTIONS END -->

### See Also

* [npm run-script](/cli/v7/commands/npm-run-script)
* [npm install](/cli/v7/commands/npm-install)
* [npm test](/cli/v7/commands/npm-test)
* [npm start](/cli/v7/commands/npm-start)
