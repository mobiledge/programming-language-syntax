# Error Handling — Gleam

```gleam
import gleam/io

fn divide(a: Float, b: Float) -> Result(Float, String) {
  case b {
    0.0 -> Error("Cannot divide by zero")
    _   -> Ok(a /. b)
  }
}

pub fn main() {
  case divide(10.0, 0.0) {
    Ok(v)    -> io.debug(v)
    Error(e) -> io.println(e)
  }
}
```
