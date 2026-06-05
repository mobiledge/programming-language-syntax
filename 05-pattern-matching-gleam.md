# Pattern Matching — Gleam

[Docs](https://tour.gleam.run/flow-control/case-expressions/)

```gleam
import gleam/io
import gleam/float

type Shape {
  Circle(radius: Float)
  Rect(width: Float, height: Float)
}

fn area(shape: Shape) -> Float {
  case shape {
    Circle(r)    -> float.pi() *. r *. r
    Rect(w, h)   -> w *. h
  }
}

pub fn main() {
  io.debug(area(Circle(5.0)))
}
```
