# Generics — Haskell

[Docs](https://wiki.haskell.org/Polymorphism)

```haskell
-- Haskell is parametrically polymorphic by default
identity :: a -> a
identity x = x

safeFirst :: [a] -> Maybe a
safeFirst []    = Nothing
safeFirst (x:_) = Just x

-- Parameterised data type
data Stack a = Stack [a]

push :: a -> Stack a -> Stack a
push x (Stack xs) = Stack (x:xs)

pop :: Stack a -> Maybe (a, Stack a)
pop (Stack [])     = Nothing
pop (Stack (x:xs)) = Just (x, Stack xs)
```
