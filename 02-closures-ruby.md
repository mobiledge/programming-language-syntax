# Closures — Ruby

```ruby
add = ->(a, b) { a + b }

result = add.call(3, 4)

# Lambda can also be invoked with .()
result = add.(3, 4)
```
