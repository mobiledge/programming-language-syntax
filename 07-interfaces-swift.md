# Interfaces / Traits — Swift

```swift
protocol Animal {
    func sound() -> String
    func describe() -> String
}

extension Animal {
    func describe() -> String { "I make a \(sound()) sound" }
}

protocol Serializable {
    func serialize() -> String
}

struct Dog: Animal, Serializable {
    func sound() -> String { "woof" }
    func serialize() -> String { #"{"type":"Dog"}"# }
}

let d: any Animal = Dog()
print(d.describe())
```
