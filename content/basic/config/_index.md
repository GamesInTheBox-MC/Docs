+++
title = "Config"
weight = 3
+++

```yaml
# Settings for games that involve blocks
block-util:
  # How many blocks to be placed for each call
  blocks-per-tick: 50

  # The delay before calling the next tick
  block-delay: 0

  # The maximum blocks to be placed (-1 for unlimited)
  max-blocks: -1

  # Should the plugin use FastAsyncWorldEdit if it exists ?
  use-fawe: true

# Settings for Planners
planner:
  # The delay between Planner's tick
  interval: 20

  # Should the planner run asynchronously ?
  async: true
```
