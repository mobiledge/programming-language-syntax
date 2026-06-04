# Interfaces / Traits — Haskell

```haskell
-- Haskell uses typeclasses as interfaces
class Animal a where
  sound    :: a -> String
  describe :: a -> String
  describe x = "I make a " ++ sound x ++ " sound"

class Serializable a where
  serialize :: a -> String

data Dog = Dog

instance Animal Dog where
  sound _ = "woof"

instance Serializable Dog where
  serialize _ = "{\"type\":\"Dog\"}"

main :: IO ()
main = putStrLn (describe Dog)
```
