# Pattern Matching — Scala

```scala
sealed trait Shape
case class Circle(radius: Double) extends Shape
case class Rect(width: Double, height: Double) extends Shape

def area(s: Shape): Double = s match
  case Circle(r)    => Math.PI * r * r
  case Rect(w, h)   => w * h

println(area(Circle(5)))
```
