# Interfaces / Traits — Ruby

[Docs](https://ruby-doc.org/core/Module.html)

```ruby
# Ruby uses modules as mixins (traits)
module Animal
  def describe
    "I make a #{sound} sound"
  end
end

module Serializable
  def serialize
    instance_variables.map { |k| [k.to_s.delete("@"), instance_variable_get(k)] }.to_h.to_json
  end
end

class Dog
  include Animal
  include Serializable

  def sound = "woof"
end

puts Dog.new.describe
```
