# Closures — TypeScript

[Docs](https://www.typescriptlang.org/docs/handbook/2/functions.html)

```typescript
function makeAdder(x: number): (y: number) => number {
  return function(y) {
    return x + y;
  };
}

const add5 = makeAdder(5);
console.log(add5(3)); // 8
```
