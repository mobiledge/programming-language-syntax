# Error Handling — Scala

[Docs](https://docs.scala-lang.org/scala3/book/fp-functional-error-handling.html)

```scala
import scala.util.{Try, Success, Failure}

def divide(a: Double, b: Double): Try[Double] =
  if b == 0 then Failure(ArithmeticException("Cannot divide by zero"))
  else Success(a / b)

divide(10, 0) match
  case Success(v) => println(s"Result: $v")
  case Failure(e) => println(s"Error: ${e.getMessage}")
```
