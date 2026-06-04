# Pattern Matching — Elixir

[Docs](https://elixir-lang.org/getting-started/pattern-matching.html)

```elixir
defmodule Shapes do
  def area({:circle, r}),      do: :math.pi() * r * r
  def area({:rect, w, h}),     do: w * h
end

IO.puts Shapes.area({:circle, 5})   # 78.53...
IO.puts Shapes.area({:rect, 3, 4})  # 12.0

# Also works inline with case
case {1, 0} do
  {0, 0} -> "Origin"
  {x, 0} -> "On x-axis at #{x}"
  {x, y} -> "Point at (#{x}, #{y})"
end
```
