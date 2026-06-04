# Interfaces / Traits — Gleam

[Docs](https://tour.gleam.run/data-types/custom-types/)

```gleam
import gleam/io

// Gleam has no interfaces; custom types +
// functions serve the same role
type Animal {
  Dog
  Cat
}

fn sound(animal: Animal) -> String {
  case animal {
    Dog -> "woof"
    Cat -> "meow"
  }
}

fn describe(animal: Animal) -> String {
  "I make a " <> sound(animal) <> " sound"
}

pub fn main() {
  io.println(describe(Dog))
}
```
