# Generics — JavaScript

[Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)

```javascript
// JavaScript has no generics; duck typing
// handles it naturally
function identity(value) {
  return value;
}

function first(arr) {
  return arr[0];
}

console.log(identity(42));       // 42
console.log(first([1, 2, 3]));  // 1
console.log(first(["a", "b"])); // "a"
```
