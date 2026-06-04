# Pattern Matching — Ruby

```ruby
# Ruby 3.0+ find pattern / deconstruct
point = { x: 1, y: 0 }

case point
in { x: 0, y: 0 }
  puts "Origin"
in { x:, y: 0 }
  puts "On x-axis at #{x}"
in { x: 0, y: }
  puts "On y-axis at #{y}"
in { x:, y: }
  puts "Point at (#{x}, #{y})"
end
```
