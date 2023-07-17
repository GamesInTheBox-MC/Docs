+++
title = "Random"
weight = 1
+++

This is a simple picker that choose a random arena from the planner.

## Format

```yaml
picker-type: random
pick-delay: <time>

settings:
  # Your game settings are generated here
```

## Note

* `pick-delay`: The time to wait before choosing the next arena

## Variable

| Variable | Description |
| --- | --- |
| `{picker_time_left}` | The time left before choosing the next arena |
