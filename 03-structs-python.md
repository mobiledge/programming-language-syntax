# Structs — Python

[Docs](https://docs.python.org/3/library/dataclasses.html)

```python
from dataclasses import dataclass

@dataclass
class Point:
    x: int
    y: int

p = Point(3, 4)
print(p.x)  # 3

# dataclasses.replace for non-destructive update
from dataclasses import replace
p2 = replace(p, x=10)
```
