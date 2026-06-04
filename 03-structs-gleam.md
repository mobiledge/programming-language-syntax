# Structs — Gleam

[Docs](https://tour.gleam.run/data-types/records/)

```gleam
// Gleam uses custom types with a single
// variant as the struct equivalent
type Point {
  Point(x: Int, y: Int)
}

let p = Point(x: 3, y: 4)
let Point(x: x_val, ..) = p
// x_val is 3

// Update via record update syntax
let p2 = Point(..p, x: 10)
```
