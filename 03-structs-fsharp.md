# Structs — F#

```fsharp
// F# uses record types as the idiomatic struct equivalent
type Point = { X: int; Y: int }

let p = { X = 3; Y = 4 }
printfn "%d" p.X // 3

// Non-destructive update
let p2 = { p with X = 10 }
```
