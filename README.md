# I am Groot
Just a CSV Util Package! keep it simple, let's groot do it for you!
# Features

Input Examples (CSV Format)
```csv
  name, height
  groot, 36.468
  another_groot, 24.128
  more_groot, 24.35
```
- **Csv file to List of Key-Value** (string, string) Dictionary
```csharp
  var iamGroots = Groot.GetDictFromCsv(path);
  
  Console.WriteLine($"Groot's height is {iamGroots[0]["height"]}");
```
- **Csv file to List of Objects**
```csharp
  #Tree
  public class Tree
  {
    public string name { get; set; }
    public decimal height { get; set; }
  }
  
  var iamGroots = Groot.GetObjectFromCsv<Tree>(path);
  Console.WriteLine($"Groot's height is {iamGroots[0].height}");
  
```
