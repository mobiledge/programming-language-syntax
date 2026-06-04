# Structs — Scala

```scala
// Scala uses case classes as the idiomatic struct equivalent
case class Point(x: Int, y: Int)

val p = Point(3, 4)
println(p.x) // 3

// Non-destructive update
val p2 = p.copy(x = 10)
```
