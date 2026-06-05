# Error Handling — Haskell

[Docs](https://wiki.haskell.org/Error_vs._Exception)

```haskell
divide :: Double -> Double -> Either String Double
divide _ 0 = Left "Cannot divide by zero"
divide a b = Right (a / b)

main :: IO ()
main = case divide 10 0 of
  Left err -> putStrLn $ "Error: " ++ err
  Right v  -> print v
```
