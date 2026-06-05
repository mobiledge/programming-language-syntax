# Enums — Kotlin

[Docs](https://kotlinlang.org/docs/enum-classes.html)

```kotlin
enum class Direction {
    NORTH, SOUTH, EAST, WEST;

    fun opposite() = when (this) {
        NORTH -> SOUTH
        SOUTH -> NORTH
        EAST  -> WEST
        WEST  -> EAST
    }
}

val d = Direction.NORTH
println(d)            // NORTH
println(d.opposite()) // SOUTH

// Sealed class for richer variants
sealed class Result
data class Success(val value: Int) : Result()
data class Failure(val error: String) : Result()
```
