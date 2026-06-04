# Error Handling — Python

[Docs](https://docs.python.org/3/tutorial/errors.html)

```python
def divide(a, b):
    if b == 0:
        raise ValueError("Cannot divide by zero")
    return a / b

try:
    result = divide(10, 0)
except ValueError as e:
    print(f"Error: {e}")
finally:
    print("Done")
```
