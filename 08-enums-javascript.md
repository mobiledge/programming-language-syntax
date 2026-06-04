# Enums — JavaScript

```javascript
// JavaScript has no built-in enums; use Object.freeze
const Direction = Object.freeze({
  NORTH: "NORTH",
  SOUTH: "SOUTH",
  EAST:  "EAST",
  WEST:  "WEST",
});

const d = Direction.NORTH;
console.log(d); // NORTH

// Check membership
console.log(Object.values(Direction).includes(d)); // true
```
