# Pattern Matching — Kotlin

[Docs](https://kotlinlang.org/docs/control-flow.html#when-expression)

```kotlin
sealed class Shape
data class Circle(val radius: Double) : Shape()
data class Rect(val width: Double, val height: Double) : Shape()

fun area(shape: Shape): Double = when (shape) {
    is Circle -> Math.PI * shape.radius * shape.radius
    is Rect   -> shape.width * shape.height
}

println(area(Circle(5.0)))
```
