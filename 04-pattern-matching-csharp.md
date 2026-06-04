# Pattern Matching — C#

```csharp
abstract record Shape;
record Circle(double Radius) : Shape;
record Rect(double Width, double Height) : Shape;

double Area(Shape s) => s switch
{
    Circle c => Math.PI * c.Radius * c.Radius,
    Rect r   => r.Width * r.Height,
    _        => throw new ArgumentException("Unknown shape")
};

Console.WriteLine(Area(new Circle(5)));
```
