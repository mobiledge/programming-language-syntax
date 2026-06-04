# Generics — Java

[Docs](https://docs.oracle.com/javase/tutorial/java/generics/)

```java
public class Stack<T> {
    private final List<T> items = new ArrayList<>();

    public void push(T item) { items.add(item); }

    public T pop() {
        return items.remove(items.size() - 1);
    }
}

// Generic method
public static <T> T first(List<T> list) {
    return list.get(0);
}

var s = new Stack<Integer>();
s.push(1);
System.out.println(s.pop()); // 1
```
