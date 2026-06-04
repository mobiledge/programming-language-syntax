# Generics — Gleam

[Docs](https://tour.gleam.run/data-types/custom-types/)

```gleam
import gleam/io

type Stack(a) {
  Stack(items: List(a))
}

fn push(stack: Stack(a), item: a) -> Stack(a) {
  Stack(items: [item, ..stack.items])
}

fn new() -> Stack(a) {
  Stack(items: [])
}

fn identity(x: a) -> a { x }

pub fn main() {
  let s = new() |> push(1) |> push(2)
  io.debug(s)
  io.debug(identity("hello"))
}
```
