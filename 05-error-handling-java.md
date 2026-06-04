# Error Handling — Java

```java
double divide(double a, double b) throws ArithmeticException {
    if (b == 0) throw new ArithmeticException("Cannot divide by zero");
    return a / b;
}

try {
    double result = divide(10, 0);
} catch (ArithmeticException e) {
    System.err.println("Error: " + e.getMessage());
} finally {
    System.out.println("Done");
}
```
