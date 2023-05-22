+++
title = "Command"
weight = 2
+++

## Main Command

* `/gitb reload`
  * **Permission**: `gamesinthebox.reload`
  * **Description**: Reload the plugin

* `/gitb action <planner> <action> [args]`
  * **Permission**: `gamesinthebox.action`
  * **Description**: Perform an action in the current arena of the planner
  * **Argument**:
    * `<planner>`: The [Planner]({{% relref "basic/definition" %}}#planner) to perform the action on the [Arena]({{% relref "basic/definition" %}}#arena)
    * `<action>`: The action to perform
    * `[args]`: The arguments required by the action
  * **Note**:
    * You can type `/gitb action <planner>` to get the list of available actions

* `/gitb end <planner>`
  * **Permission**: `gamesinthebox.end`
  * **Description**: Force the planner to end the current arena of the planner
  * **Argument**:
    * `<planner>`: The [Planner]({{% relref "basic/definition" %}}#planner) to end the current [Arena]({{% relref "basic/definition" %}}#arena)

* `/gitb forcepick <planner>`
  * **Permission**: `gamesinthebox.forcepick`
  * **Description**: Force the planner to pick the next arena
  * **Argument**:
    * `<planner>`: The [Planner]({{% relref "basic/definition" %}}#planner) to force the picker

* `/gitb setgame <planner> <arena>`
  * **Permission**: `gamesinthebox.setgame`
  * **Description**: Set the next arena in the planner
  * **Argument**:
    * `<planner>`: The [Planner]({{% relref "basic/definition" %}}#planner) to pick the [Arena]({{% relref "basic/definition" %}}#arena)
    * `<arena>`: The [Arena]({{% relref "basic/definition" %}}#arena) to choose for the [Planner]({{% relref "basic/definition" %}}#planner)

* `/gitb expansion`
  * **Permission**: `gamesinthebox.expansion`
  * **Description**: Get the running expansions of the plugin

## Editor Command

> Permission: `gamesinthebox.editor`

* `/gitbeditor usage <game>`
  * **Description**: Get the usage of the editor. It's usually about the available actions that can be performed on the editor
  * **Argument**:
    * `<game>`: The [Game]({{% relref "basic/definition" %}}#game) to edit

* `/gitbeditor save <game> <planner> <arena> [override]`
  * **Description**: Save the settings of the game to the planner as an arena
  * **Argument**:
    * `<game>`: The [Game]({{% relref "basic/definition" %}}#game) to save
    * `<planner>`: The [Planner]({{% relref "basic/definition" %}}#planner) that the [Game]({{% relref "basic/definition" %}}#game) would be saved to
    * `<arena>`: The name of the [Arena]({{% relref "basic/definition" %}}#arena) that the [Game]({{% relref "basic/definition" %}}#game) would be saved as
    * `[override]`: Whether to override current settings if the [Arena]({{% relref "basic/definition" %}}#arena) exists. Default to `false` if not specified

* `/gitbeditor action <game> <action> [args]`
  * **Description**: Perform an action on the editor
  * **Argument**:
    * `<game>`: The [Game]({{% relref "basic/definition" %}}#game) to perform the action
    * `<action>`: The action to perform
    * `[args]`: The arguments required by the action

* `/gitbeditor reset <game>`
  * **Description**: Reset the editor
  * **Argument**:
    * `<game>`: The [Game]({{% relref "basic/definition" %}}#game) to edit

* `/gitbeditor status <game>`
  * **Description**: Get the status of the editor
  * **Argument**:
    * `<game>`: The [Game]({{% relref "basic/definition" %}}#game) to edit

* `/gitbeditor migrate <game> <planner> <arena>`
  * **Description**: Migrate the settings from an arena
  * **Argument**:
    * `<game>`: The [Game]({{% relref "basic/definition" %}}#game) to migrate the settings
    * `<planner>`: The [Planner]({{% relref "basic/definition" %}}#planner) that has the [Arena]({{% relref "basic/definition" %}}#arena) to migrate to
    * `<arena>`: The [Arena]({{% relref "basic/definition" %}}#arena) to migrate the settings to
