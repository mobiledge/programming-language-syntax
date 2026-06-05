# Enums — TypeScript

[Docs](https://www.typescriptlang.org/docs/handbook/enums.html)

```typescript
// String enum
enum Direction {
  North = "NORTH",
  South = "SOUTH",
  East  = "EAST",
  West  = "WEST",
}

const d: Direction = Direction.North;
console.log(d); // NORTH

// Const enum (erased at compile time)
const enum Color { Red, Green, Blue }
const c = Color.Red; // compiles to 0
```
