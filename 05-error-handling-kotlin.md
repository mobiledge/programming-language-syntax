# Error Handling — Kotlin

```kotlin
// Kotlin: runCatching returns a Result<T>
fun divide(a: Double, b: Double): Double {
    require(b != 0.0) { "Cannot divide by zero" }
    return a / b
}

val result = runCatching { divide(10.0, 0.0) }
result
    .onSuccess { println("Result: $it") }
    .onFailure { println("Error: ${it.message}") }
```
