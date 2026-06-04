# Pattern Matching — Java

```java
// Java 21 pattern matching in switch
sealed interface Shape permits Circle, Rect {}
record Circle(double radius) implements Shape {}
record Rect(double width, double height) implements Shape {}

double area(Shape s) {
    return switch (s) {
        case Circle c -> Math.PI * c.radius() * c.radius();
        case Rect r   -> r.width() * r.height();
    };
}
```
