# Generics — Elixir

[Docs](https://elixir-lang.org/getting-started/typespecs-and-behaviours.html)

```elixir
# Elixir is dynamically typed; functions work on any type naturally
defmodule Stack do
  def new,          do: []
  def push(s, item), do: [item | s]
  def pop([h | t]), do: {h, t}
end

defmodule Utils do
  def first([h | _]), do: h
  def first([]),      do: nil
end

s = Stack.new() |> Stack.push(1) |> Stack.push(2)
{top, rest} = Stack.pop(s)
IO.puts top           # 2
IO.puts Utils.first([1, 2, 3])  # 1
```
