# Enums — Gleam

[Docs](https://tour.gleam.run/data-types/custom-types/)

```gleam
import gleam/io

type Direction {
  North
  South
  East
  West
}

fn opposite(d: Direction) -> Direction {
  case d {
    North -> South
    South -> North
    East  -> West
    West  -> East
  }
}

// Custom type with data (like enum variants with values)
type Result(value, error) {
  Ok(value)
  Error(error)
}

pub fn main() {
  io.debug(opposite(North))  // South
}
```
