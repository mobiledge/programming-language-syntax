# Closures — Swift

[Docs](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/closures/)

```swift
let add = { (a: Int, b: Int) -> Int in
    return a + b
}

let result = add(3, 4)

// Shorthand: Swift can infer types and uses $0, $1 for arguments
let addShort: (Int, Int) -> Int = { $0 + $1 }
```
