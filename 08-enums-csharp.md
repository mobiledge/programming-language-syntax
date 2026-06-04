# Enums — C#

[Docs](https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/enum)

```csharp
enum Direction { North, South, East, West }

// Flags enum (bitwise)
[Flags]
enum Permission { None = 0, Read = 1, Write = 2, Execute = 4 }

Direction d = Direction.North;
Console.WriteLine(d);       // North
Console.WriteLine((int)d);  // 0

var perms = Permission.Read | Permission.Write;
Console.WriteLine(perms);   // Read, Write
```
