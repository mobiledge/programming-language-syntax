# Structs — Elixir

```elixir
# Elixir structs are defined inside a module
defmodule Point do
  defstruct x: 0, y: 0
end

p = %Point{x: 3, y: 4}
IO.inspect(p.x) # 3

# Update a field (returns a new struct)
p2 = %Point{p | x: 10}
```
