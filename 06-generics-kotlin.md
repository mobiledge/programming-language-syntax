# Generics — Kotlin

[Docs](https://kotlinlang.org/docs/generics.html)

```kotlin
class Stack<T> {
    private val items = mutableListOf<T>()
    fun push(item: T) = items.add(item)
    fun pop(): T = items.removeLast()
}

fun <T> first(list: List<T>): T = list.first()

val s = Stack<Int>()
s.push(1)
println(s.pop()) // 1
println(first(listOf("a", "b"))) // a
```
