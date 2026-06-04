# Enums — Python

[Docs](https://docs.python.org/3/library/enum.html)

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
