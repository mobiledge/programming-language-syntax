# Interfaces / Traits — TypeScript

[Docs](https://www.typescriptlang.org/docs/handbook/2/objects.html#interfaces)

```typescript
interface Animal {
  sound(): string;
  describe(): string;
}

interface Serializable {
  serialize(): string;
}

class Dog implements Animal, Serializable {
  sound() { return "woof"; }
  describe() { return `I make a ${this.sound()} sound`; }
  serialize() { return JSON.stringify({ type: "Dog" }); }
}

const d: Animal = new Dog();
console.log(d.describe());
```
