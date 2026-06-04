# Pattern Matching — JavaScript

[Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment)

```javascript
// JavaScript has no native pattern matching; destructuring + conditionals
function describe(point) {
  const { x, y } = point;
  if (x === 0 && y === 0) return "Origin";
  if (y === 0) return `On x-axis at ${x}`;
  if (x === 0) return `On y-axis at ${y}`;
  return `Point at (${x}, ${y})`;
}

console.log(describe({ x: 1, y: 0 })); // On x-axis at 1
```
