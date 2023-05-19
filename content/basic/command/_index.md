+++
title = "Command"
weight = 2
+++

## Main Command

| Command | Permission | Description |
| --- | --- | --- |
| `/gitb reload` | `gamesinthebox.reload` | Reload the plugin |
| `/gitb action <planner> <action> [args]` | `gamesinthebox.action` | Perform actions in the current arena of the planner |
| `/gitb end <planner>` | `gamesinthebox.end` | Force the planner to end the current arena of the planner |
| `/gitb forcepick <planner>` | `gamesinthebox.forcepick` | Force the planner to pick the next arena |
| `/gitb setgame <planner> <arena>` | `gamesinthebox.setgame` | Set the next arena in the planner |
| `/gitb expansion` | `gamesinthebox.expansion` | Get the running expansions of the plugin |

## Editor Command

> Permission: `gamesinthebox.editor`

| Command | Description |
| --- | --- |
| `/gitbeditor usage <game>` | Get the usage of the editor |
| `/gitbeditor save <game> <planner> <arena> [override]` | Save the settings to the planner |
| `/gitbeditor action <game> <action> [args]` | Perform an action on the editor |
| `/gitbeditor reset <game>` | Reset the editor |
| `/gitbeditor status <game>` | Get the status of the editor |
| `/gitbeditor migrate <game> <planner> <arena>` | Migrate the settings from a game arena |
