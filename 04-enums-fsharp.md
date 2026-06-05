# Enums — F#

[Docs](https://learn.microsoft.com/en-us/dotnet/fsharp/language-reference/discriminated-unions)

```fsharp
// Simple enum
type Direction = North | South | East | West

let opposite = function
    | North -> South
    | South -> North
    | East  -> West
    | West  -> East

// Discriminated union (richer variant)
type Result<'T> =
    | Success of 'T
    | Failure of string

printfn "%A" North               // North
printfn "%A" (opposite North)    // South
printfn "%A" (Success 42)
// Success 42
```
