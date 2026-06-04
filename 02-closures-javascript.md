# Closures — JavaScript

[Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures)

```javascript
function makeAdder(x) {
  return function(y) {
    return x + y;
  };
}

const add5 = makeAdder(5);
console.log(add5(3)); // 8
```
