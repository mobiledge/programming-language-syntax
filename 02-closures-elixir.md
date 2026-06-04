# Closures — Elixir

[Docs](https://elixir-lang.org/getting-started/modules-and-functions.html#function-capturing)

```elixir
add = fn a, b -> a + b end

result = add.(3, 4)

# Note: anonymous functions require a dot before the parentheses when invoked
```
