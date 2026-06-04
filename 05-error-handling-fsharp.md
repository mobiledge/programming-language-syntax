# Error Handling — F#

[Docs](https://learn.microsoft.com/en-us/dotnet/fsharp/language-reference/exception-handling/)

```fsharp
let divide a b =
    if b = 0.0 then Error "Cannot divide by zero"
    else Ok (a / b)

match divide 10.0 0.0 with
| Ok v    -> printfn "Result: %f" v
| Error e -> printfn "Error: %s" e
```
