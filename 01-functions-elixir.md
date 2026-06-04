# Functions — Elixir

```elixir
# Named functions must be defined inside a module
defmodule Math do
  def add(a, b) do
    a + b  # last expression is implicitly returned
  end
end

result = Math.add(3, 4)
```
