# Closures — TypeScript

```typescript
function makeAdder(x: number): (y: number) => number {
  return function(y) {
    return x + y;
  };
}

const add5 = makeAdder(5);
console.log(add5(3)); // 8
```
