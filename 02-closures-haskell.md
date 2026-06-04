# Closures — Haskell

[Docs](https://wiki.haskell.org/Closure)

```haskell
-- Lambda syntax uses backslash to evoke λ
add :: Int -> Int -> Int
add = \a b -> a + b

result = add 3 4
```
