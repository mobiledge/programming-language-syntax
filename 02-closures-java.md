# Closures — Java

[Docs](https://docs.oracle.com/javase/tutorial/java/javaOO/lambdaexpressions.html)

```java
// Java uses lambdas via functional interfaces; BiFunction is the standard two-arg interface
import java.util.function.BiFunction;

BiFunction<Integer, Integer, Integer> add = (a, b) -> a + b;

int result = add.apply(3, 4);
```
