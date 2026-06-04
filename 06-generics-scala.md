# Generics — Scala

[Docs](https://docs.scala-lang.org/scala3/book/types-generics.html)

```scala
class Stack[T]:
  private var items: List[T] = Nil
  def push(item: T): Unit = items = item :: items
  def pop(): T = { val h = items.head; items = items.tail; h }

def first[T](list: List[T]): T = list.head

val s = Stack[Int]()
s.push(1)
println(s.pop())           // 1
println(first(List(1, 2))) // 1
```
