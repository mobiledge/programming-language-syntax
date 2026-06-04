# Enums — Java

[Docs](https://docs.oracle.com/javase/tutorial/java/javaOO/enum.html)

```java
enum Direction {
    NORTH, SOUTH, EAST, WEST;

    public Direction opposite() {
        return switch (this) {
            case NORTH -> SOUTH;
            case SOUTH -> NORTH;
            case EAST  -> WEST;
            case WEST  -> EAST;
        };
    }
}

Direction d = Direction.NORTH;
System.out.println(d);            // NORTH
System.out.println(d.opposite()); // SOUTH
```
