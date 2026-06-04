# Structs — Haskell

[Docs](https://wiki.haskell.org/Record_syntax)

```haskell
-- Haskell uses data types with record syntax as the struct equivalent
data Point = Point
  { x :: Int
  , y :: Int
  } deriving (Show)

p :: Point
p = Point { x = 3, y = 4 }

-- Access a field
main :: IO ()
main = do
  print (x p)   -- 3

  -- Non-destructive update
  let p2 = p { x = 10 }
  print p2      -- Point {x = 10, y = 4}
```
