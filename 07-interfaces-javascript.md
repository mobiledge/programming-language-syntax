# Interfaces / Traits — JavaScript

```javascript
// JavaScript has no interfaces; duck typing and mixins are used
const Serializable = (Base) => class extends Base {
  serialize() { return JSON.stringify(this); }
};

class User extends Serializable(class {}) {
  constructor(name) { super(); this.name = name; }
}

const u = new User("Alice");
console.log(u.serialize()); // {"name":"Alice"}
```
