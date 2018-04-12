# ConsoleTable

> #### Options
> ```ConsoleTableOptions.Pad```           := Is the Length of each cell.  
> ```ConsoleTableOptions.DefaultIfNull``` := If the cell is null, set the default value

## Example:

```csharp
  var header = new List<string>{ "Coluna 1", "Coluna 2" };
  var row = new List<string>{ "Row 1", "Row 2" };
  
  var table = new ConsoleTable(header, row);
  
  var newRow1 = new [] {"value1", "value2"};
  var newRow2 = new [] {"value3", "value4"};
  var newRow3 = new [] {"value5", "value6"};
  
  table.AddRow(newRow1);
  table.AddRow(newRow2);
  table.AddRow(newRow3);
  
  table.Write();
```
