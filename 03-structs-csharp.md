# Structs — C#

```csharp
struct Point
{
    public int X;
    public int Y;

    public Point(int x, int y)
    {
        X = x;
        Y = y;
    }
}

var p = new Point(3, 4);
Console.WriteLine(p.X); // 3
```
