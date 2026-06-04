# Error Handling — JavaScript

[Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Control_flow_and_error_handling#exception_handling_statements)

```javascript
function divide(a, b) {
  if (b === 0) throw new Error("Cannot divide by zero");
  return a / b;
}

try {
  const result = divide(10, 0);
} catch (err) {
  console.error("Error:", err.message);
} finally {
  console.log("Done");
}
```
