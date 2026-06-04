# Generics — C#

[Docs](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/types/generics)

```csharp
class Stack<T>
{
    private readonly List<T> items = new();

    public void Push(T item) => items.Add(item);
    public T Pop() { var v = items[^1]; items.RemoveAt(items.Count - 1); return v; }
}

T First<T>(IList<T> list) => list[0];

var s = new Stack<int>();
s.Push(1);
Console.WriteLine(s.Pop()); // 1
Console.WriteLine(First(new[] { "a", "b" })); // a
```
