# Generics — Ruby

[Docs](https://ruby-doc.org/core/Array.html)

```ruby
# Ruby is dynamically typed; all containers
# are generic by default
class Stack
  def initialize = @items = []
  def push(item) = @items.push(item)
  def pop        = @items.pop
end

def first(arr) = arr.first

s = Stack.new
s.push(1)
puts s.pop          # 1
puts first(%w[a b]) # a
```
