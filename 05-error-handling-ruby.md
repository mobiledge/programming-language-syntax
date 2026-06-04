# Error Handling — Ruby

[Docs](https://ruby-doc.org/core/Exception.html)

```ruby
def divide(a, b)
  raise ArgumentError, "Cannot divide by zero" if b == 0
  a.to_f / b
end

begin
  result = divide(10, 0)
rescue ArgumentError => e
  puts "Error: #{e.message}"
ensure
  puts "Done"
end
```
