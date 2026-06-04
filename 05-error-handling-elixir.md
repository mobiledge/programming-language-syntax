# Error Handling — Elixir

```elixir
defmodule Math do
  def divide(_a, 0), do: {:error, "Cannot divide by zero"}
  def divide(a, b),  do: {:ok, a / b}
end

case Math.divide(10, 0) do
  {:ok, result}    -> IO.puts("Result: #{result}")
  {:error, reason} -> IO.puts("Error: #{reason}")
end
```
