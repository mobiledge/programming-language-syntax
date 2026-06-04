# Enums — Elixir

```elixir
# Elixir uses atoms as enum values; modules group related atoms
defmodule Direction do
  @north :north
  @south :south
  @east  :east
  @west  :west

  def all, do: [@north, @south, @east, @west]

  def opposite(:north), do: :south
  def opposite(:south), do: :north
  def opposite(:east),  do: :west
  def opposite(:west),  do: :east
end

IO.inspect Direction.all()            # [:north, :south, :east, :west]
IO.inspect Direction.opposite(:north) # :south
```
