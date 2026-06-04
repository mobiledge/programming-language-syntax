# Pattern Matching — Haskell

```haskell
data Shape = Circle Double | Rect Double Double

area :: Shape -> Double
area (Circle r)  = pi * r * r
area (Rect w h)  = w * h

main :: IO ()
main = do
  print (area (Circle 5))   -- 78.53...
  print (area (Rect 3 4))   -- 12.0
```
