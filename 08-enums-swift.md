# Enums — Swift

```swift
enum Direction {
    case north, south, east, west

    var opposite: Direction {
        switch self {
        case .north: return .south
        case .south: return .north
        case .east:  return .west
        case .west:  return .east
        }
    }
}

// Enums with associated values
enum Result {
    case success(Int)
    case failure(String)
}

let d = Direction.north
print(d.opposite) // south

let r = Result.success(42)
if case .success(let v) = r { print(v) } // 42
```
