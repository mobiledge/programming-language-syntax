# Pattern Matching — Swift

[Docs](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/patterns/)

```swift
enum Shape {
    case circle(radius: Double)
    case rect(width: Double, height: Double)
}

func area(_ shape: Shape) -> Double {
    switch shape {
    case .circle(let r):      return .pi * r * r
    case .rect(let w, let h): return w * h
    }
}

print(area(.circle(radius: 5)))
```
