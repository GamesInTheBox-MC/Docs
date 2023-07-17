+++
title = "Chance"
weight = 2
+++

This is a picker that choose a random arena based on the specific chance of it.

## Format

```yaml
picker-type: chance
pick-delay: <time>
pick-chance:
  arena1: 10
  arena2: 20
  arena3: 30
  arena4: 40

settings:
  # Your game settings are generated here
```

## Note

* `pick-delay`: The time to wait before choosing the next arena
* `pick-chance`: The chance that an arena would be picked

## Variable

| Variable | Description |
| --- | --- |
| `{picker_time_left}` | The time left before choosing the next arena |
