# Structs — Scala

[Docs](https://docs.scala-lang.org/scala3/book/domain-modeling-tools.html)

```scala
// Scala uses case classes as the idiomatic
// struct equivalent
case class Point(x: Int, y: Int)

val p = Point(3, 4)
println(p.x) // 3

// Non-destructive update
val p2 = p.copy(x = 10)
```
