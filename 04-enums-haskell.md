# Enums — Haskell

[Docs](https://wiki.haskell.org/Algebraic_data_type)

```haskell
data Direction = North | South | East | West
  deriving (Show, Eq, Ord, Enum, Bounded)

opposite :: Direction -> Direction
opposite North = South
opposite South = North
opposite East  = West
opposite West  = East

main :: IO ()
main = do
  print North              -- North
  print (opposite North)   -- South
  print [minBound..maxBound :: Direction]
  -- [North,South,East,West]
```
