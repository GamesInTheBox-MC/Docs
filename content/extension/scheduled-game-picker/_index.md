+++
title = "Scheduled Game Picker"
weight = 1
+++

{{% button href="https://github.com/GamesInTheBox-MC/ScheduledGamePicker/releases" style="green" icon="download" %}}Download{{% /button %}}

This is a picker that choose an arena based on a specific set of time events.

## Install

1. Go to [the download page](https://github.com/GamesInTheBox-MC/ScheduledGamePicker/releases)
2. Choose the latest version
3. Download the `-shaded` file
4. Copy the downloaded file to the folder `plugins/GamesInTheBox/expansions`
5. Restart the server

## Format

```yaml
picker-type: cron
pick-time:
  arena1: "* 10 0 ? * * *"
  arena2: "* 20 0 ? * * *"
  arena3: "* 30 0 ? * * *"

settings:
  # Your game settings are generated here
```

## Note

* `pick-time`: The pair of the arena name and a Cron expression that describes how often the arena takes part in

{{% notice style="tip" %}}
You can go to [this page](https://www.freeformatter.com/cron-expression-generator-quartz.html) to generate a Cron expression.
{{% /notice %}}

## Variable

| Variable | Description |
| --- | --- |
| `{picker_time_left}` | The time left before choosing the next arena |
| `{picker_next_game_name}` | The display name of the game of the next arena |
