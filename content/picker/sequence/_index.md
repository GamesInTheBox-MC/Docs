+++
title = "Sequence"
weight = 3
+++

This is a picker that choose an arena in the specific sequence of arenas.

## Format

```yaml
picker-type: sequence
pick-delay: <time>
pick-sequence:
  - "arena1,arena2,arena3"
  - "arena4,arena5"
  - "arena6"

settings:
  # Your game settings are generated here
```

## Note

* `pick-delay`: The time to wait before choosing the next arena
* `pick-sequence`: The sequence of arenas (as a list) that the picker would follow along with

{{% notice style="tip" %}}
The picker would follow the sequence line-by-line. However, you can add multiple arenas in a line and let the picker randomly choose one of them.

```yaml
pick-sequence:
  - "arena1,arena2,arena3" # 1. Play one of arena1, arena2, arena3
  - "arena4,arena5"        # 2. Play one of arena4, arena5
  - "arena6"               # 3. Play arena6
```
{{% /notice %}}

## Variable

| Variable | Description |
| --- | --- |
| `{picker_time_left}` | The time left before choosing the next arena |
