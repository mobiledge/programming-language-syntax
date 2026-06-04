# Pattern Matching — Python

[Docs](https://docs.python.org/3/reference/compound_stmts.html#the-match-statement)

```python
# Python 3.10+ match/case
point = (1, 0)

match point:
    case (0, 0):
        print("Origin")
    case (x, 0):
        print(f"On x-axis at {x}")
    case (0, y):
        print(f"On y-axis at {y}")
    case (x, y):
        print(f"Point at ({x}, {y})")
```
