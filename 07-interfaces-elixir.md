# Interfaces / Traits — Elixir

```elixir
# Elixir uses behaviours as interfaces and protocols for polymorphism
defmodule Animal do
  @callback sound() :: String.t()
end

defmodule Dog do
  @behaviour Animal
  def sound(), do: "woof"
  def describe(), do: "I make a #{sound()} sound"
end

# Protocols for ad-hoc polymorphism
defprotocol Serializable do
  def serialize(value)
end

defimpl Serializable, for: Map do
  def serialize(m), do: Jason.encode!(m)
end
```
