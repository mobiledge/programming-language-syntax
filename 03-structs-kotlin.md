# Structs — Kotlin

[Docs](https://kotlinlang.org/docs/data-classes.html)

```kotlin
// Kotlin uses data classes as the idiomatic
// struct equivalent
data class Point(val x: Int, val y: Int)

val p = Point(3, 4)
println(p.x) // 3

// Non-destructive update
val p2 = p.copy(x = 10)
```
