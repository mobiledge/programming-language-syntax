# Pattern Matching — F#

```fsharp
type Shape =
    | Circle of radius: float
    | Rect of width: float * height: float

let area shape =
    match shape with
    | Circle r    -> System.Math.PI * r * r
    | Rect (w, h) -> w * h

printfn "%f" (area (Circle 5.0))
printfn "%f" (area (Rect (3.0, 4.0)))
```
