# Structs — Swift

```swift
struct Point {
    var x: Int
    var y: Int
}

var p = Point(x: 3, y: 4)
print(p.x) // 3

// Structs are value types — assignment copies
var p2 = p
p2.x = 10
// p.x is still 3
```
