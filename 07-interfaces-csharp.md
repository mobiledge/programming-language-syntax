# Interfaces / Traits — C#

```csharp
interface IAnimal
{
    string Sound();
    string Describe() => $"I make a {Sound()} sound"; // default implementation
}

interface ISerializable
{
    string Serialize();
}

class Dog : IAnimal, ISerializable
{
    public string Sound() => "woof";
    public string Serialize() => """{"type":"Dog"}""";
}

IAnimal d = new Dog();
Console.WriteLine(d.Describe());
```
