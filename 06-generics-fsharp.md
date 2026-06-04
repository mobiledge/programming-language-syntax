# Generics — F#

[Docs](https://learn.microsoft.com/en-us/dotnet/fsharp/language-reference/generics/)

```fsharp
// F# infers generic type parameters
// automatically
let identity x = x

let safeFirst = function
    | [] -> None
    | x :: _ -> Some x

type Stack<'T> = Stack of 'T list

let push item (Stack items) = Stack (item :: items)
let pop (Stack items) =
    match items with
    | []     -> None, Stack []
    | x :: rest -> Some x, Stack rest

let s = Stack [] |> push 1 |> push 2
printfn "%A" s  // Stack [2; 1]
```
