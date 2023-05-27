+++
title = "Variable"
weight = 4
+++

The plugin provides built-in variables for Game, Arena & Game. These variables can be used in game messages and actions.

## Built-in variables

| Variable | Description |
| --- | --- |
| `{planner_name}` | The name of the planner |
| `{planner_game_name}` | The display name of the game of the current arena of the planner |
| `{planner_game_local_name}` | The name of the current arena of the planner |
| `{planner_state}` | The current state of the planner |
| `{planner_game_state}` | The state of the current arena of the planner |

## Hook to PlaceholderAPI

The variables can be used in PlaceholderAPI with this format:

```
%gamesinthebox_<planner>:<variable>%
```

- `<planner>` is the name of the planner to request
- `<variable>` is the plugin variable without curly brackets `{}`

For example, if you want to get the `{planner_game_state}` of a planner named `my_game`, the placeholder for that will be

```
%gamesinthebox_my_game:planner_game_state%
```
