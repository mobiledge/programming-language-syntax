# Error Handling — TypeScript

[Docs](https://www.typescriptlang.org/docs/handbook/2/types-from-types.html)

```typescript
// TypeScript: Result-style type for typed errors
type Result<T, E> = { ok: true; value: T } | { ok: false; error: E };

function divide(a: number, b: number): Result<number, string> {
  if (b === 0) return { ok: false, error: "Cannot divide by zero" };
  return { ok: true, value: a / b };
}

const res = divide(10, 0);
if (!res.ok) console.error(res.error);
else console.log(res.value);
```
