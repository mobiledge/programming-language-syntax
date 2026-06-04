# Interfaces / Traits — Python

[Docs](https://docs.python.org/3/library/abc.html)

```python
from abc import ABC, abstractmethod

class Animal(ABC):
    @abstractmethod
    def sound(self) -> str: ...

    def describe(self) -> str:
        return f"I make a {self.sound()} sound"

class Dog(Animal):
    def sound(self) -> str:
        return "woof"

# Protocol (structural typing, no inheritance needed)
from typing import Protocol

class Drawable(Protocol):
    def draw(self) -> None: ...
```
