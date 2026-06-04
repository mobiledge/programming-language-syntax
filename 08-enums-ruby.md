# Enums — Ruby

[Docs](https://ruby-doc.org/core/Symbol.html)

```ruby
# Ruby has no built-in enums; symbols or constants are conventional
module Direction
  NORTH = :north
  SOUTH = :south
  EAST  = :east
  WEST  = :west

  ALL = [NORTH, SOUTH, EAST, WEST].freeze
end

d = Direction::NORTH
puts d        # north
puts d.upcase # NORTH
puts Direction::ALL.inspect
```
