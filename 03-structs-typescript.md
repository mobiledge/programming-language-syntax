# Structs — TypeScript

```typescript
// TypeScript uses interfaces or type aliases as the struct equivalent
interface Point {
  x: number;
  y: number;
}

const p: Point = { x: 3, y: 4 };
console.log(p.x); // 3

// Non-destructive update via spread
const p2: Point = { ...p, x: 10 };
```
