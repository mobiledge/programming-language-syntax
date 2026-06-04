# Structs — Java

[Docs](https://docs.oracle.com/en/java/javase/16/language/records.html)

```java
// Java uses records (Java 16+) as the
// idiomatic struct equivalent
record Point(int x, int y) {}

var p = new Point(3, 4);
System.out.println(p.x()); // 3
```
