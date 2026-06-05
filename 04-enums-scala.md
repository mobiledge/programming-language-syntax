# Enums — Scala

[Docs](https://docs.scala-lang.org/scala3/book/types-adts-gadts.html)

```scala
// Scala 3 enum
enum Direction:
  case North, South, East, West

  def opposite: Direction = this match
    case North => South
    case South => North
    case East  => West
    case West  => East

val d = Direction.North
println(d)            // North
println(d.opposite)   // South

// Enum with parameters
enum Color(val hex: String):
  case Red   extends Color("#FF0000")
  case Green extends Color("#00FF00")
  case Blue  extends Color("#0000FF")
```
