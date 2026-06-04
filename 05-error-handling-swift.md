# Error Handling — Swift

[Docs](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/errorhandling/)

```swift
enum MathError: Error {
    case divisionByZero
}

func divide(_ a: Double, _ b: Double) throws -> Double {
    guard b != 0 else { throw MathError.divisionByZero }
    return a / b
}

do {
    let result = try divide(10, 0)
    print(result)
} catch MathError.divisionByZero {
    print("Error: Cannot divide by zero")
}
```
