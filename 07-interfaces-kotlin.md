# Interfaces / Traits — Kotlin

[Docs](https://kotlinlang.org/docs/interfaces.html)

```kotlin
interface Animal {
    fun sound(): String
    fun describe() = "I make a ${sound()} sound"
}

interface Serializable {
    fun serialize(): String
}

class Dog : Animal, Serializable {
    override fun sound() = "woof"
    override fun serialize() = """{"type":"Dog"}"""
}

val d: Animal = Dog()
println(d.describe())
```
