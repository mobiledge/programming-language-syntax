# Interfaces / Traits — Scala

[Docs](https://docs.scala-lang.org/scala3/book/domain-modeling-tools.html#traits)

```scala
trait Animal:
  def sound(): String
  def describe(): String = s"I make a ${sound()} sound"

trait Serializable:
  def serialize(): String

class Dog extends Animal with Serializable:
  def sound() = "woof"
  def serialize() = """{"type":"Dog"}"""

val d: Animal = Dog()
println(d.describe())
```
