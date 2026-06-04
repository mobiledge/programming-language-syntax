# Enums — Python

```python
from enum import Enum, auto

class Direction(Enum):
    NORTH = auto()
    SOUTH = auto()
    EAST  = auto()
    WEST  = auto()

d = Direction.NORTH
print(d)        # Direction.NORTH
print(d.name)   # NORTH
print(d.value)  # 1

for direction in Direction:
    print(direction)
```
