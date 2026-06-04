# Interfaces / Traits — Java

[Docs](https://docs.oracle.com/javase/tutorial/java/IandI/createinterface.html)

```java
interface Animal {
    String sound();

    default String describe() {
        return "I make a " + sound() + " sound";
    }
}

interface Serializable {
    String serialize();
}

class Dog implements Animal, Serializable {
    public String sound() { return "woof"; }
    public String serialize() { return "{\"type\":\"Dog\"}"; }
}

Animal d = new Dog();
System.out.println(d.describe());
```
