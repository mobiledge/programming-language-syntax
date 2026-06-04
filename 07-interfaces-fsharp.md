# Interfaces / Traits — F#

[Docs](https://learn.microsoft.com/en-us/dotnet/fsharp/language-reference/interfaces)

```fsharp
type IAnimal =
    abstract member Sound: unit -> string
    abstract member Describe: unit -> string

type ISerializable =
    abstract member Serialize: unit -> string

type Dog() =
    interface IAnimal with
        member _.Sound() = "woof"
        member this.Describe() = $"I make a {(this :> IAnimal).Sound()} sound"
    interface ISerializable with
        member _.Serialize() = """{"type":"Dog"}"""

let d = Dog() :> IAnimal
printfn "%s" (d.Describe())
```
