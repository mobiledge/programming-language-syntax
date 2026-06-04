# Generics — Swift

```swift
struct Stack<T> {
    private var items: [T] = []
    mutating func push(_ item: T) { items.append(item) }
    mutating func pop() -> T?    { items.popLast() }
}

func first<T>(_ array: [T]) -> T? { array.first }

var s = Stack<Int>()
s.push(1)
print(s.pop()!)        // 1
print(first([1, 2])!)  // 1
```
