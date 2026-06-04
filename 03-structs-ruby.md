# Structs — Ruby

[Docs](https://ruby-doc.org/core/Struct.html)

```ruby
Point = Data.define(:x, :y)
# Ruby 3.2+ immutable struct

p = Point.new(x: 3, y: 4)
puts p.x  # 3

# Non-destructive update
p2 = p.with(x: 10)
```
