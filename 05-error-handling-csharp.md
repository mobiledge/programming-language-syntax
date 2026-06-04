# Error Handling — C#

```csharp
double Divide(double a, double b)
{
    if (b == 0) throw new DivideByZeroException("Cannot divide by zero");
    return a / b;
}

try
{
    double result = Divide(10, 0);
}
catch (DivideByZeroException ex)
{
    Console.Error.WriteLine($"Error: {ex.Message}");
}
finally
{
    Console.WriteLine("Done");
}
```
