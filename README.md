# Qlik Sense / QlikView Syntax for VS Code

Syntax highlighting and code snippets for Qlik Sense and QlikView script files (`.qvs`) in Visual Studio Code.

Based on the official Qlik Sense November 2026 SR2 BNF grammar specification.

## Features

- **Full syntax highlighting** for 433+ functions across 24 categories
- **552 code snippets** with parameter placeholders
- **Auto-closing pairs** for brackets, quotes, and comments
- **Code folding** support with `// #region` / `// #endregion` markers
- **Indentation rules** for control structures

## Supported Categories

| Category | Count | Examples |
|----------|-------|---------|
| Aggregation | 90 | `Sum`, `Count`, `Avg`, `Max`, `Min`, `Correl`, `Fractile` |
| Date & Time | 68 | `Year`, `Month`, `Day`, `Now`, `Today`, `AddMonths` |
| Probability & Statistics | 76 | `NormDist`, `TTest_*`, `ZTest_*`, `LinEst_*` |
| String | 48 | `Upper`, `Lower`, `Trim`, `Replace`, `Mid`, `Len` |
| Color | 25 | `RGB`, `ARGB`, `HSL`, `Red`, `Blue`, `Green` |
| Range | 24 | `RangeSum`, `RangeAvg`, `RangeMax`, `RangeMin` |
| System | 18 | `OSUser`, `ComputerName`, `ReloadTime`, `DocumentName` |
| File | 15 | `FileSize`, `FileName`, `FilePath`, `Attribute` |
| Financial | 14 | `FV`, `PV`, `Pmt`, `Rate`, `Irr`, `Npv` |
| Numeric Interpretation | 14 | `Date`, `Num`, `Money`, `Time`, `Dual` |
| Numeric | 13 | `Ceil`, `Floor`, `Round`, `Mod`, `Div` |
| Trigonometric | 13 | `Sin`, `Cos`, `Tan`, `Acos`, `Asin`, `Atan` |
| Conditional | 12 | `If`, `Alt`, `Match`, `Pick`, `Coalesce` |
| Geo | 10 | `GeoMakePoint`, `GeoProject`, `GeoBoundingBox` |
| Table | 10 | `FieldName`, `FieldValue`, `NoOfRows`, `NoOfTables` |
| Legacy (deprecated) | 9 | `NumAvg`, `NumSum`, `QVUser` |
| Logical | 7 | `IsNull`, `IsNum`, `IsText`, `True`, `False` |
| Exponential | 6 | `Exp`, `Log`, `Log10`, `Pow`, `Sqr`, `Sqrt` |
| Counter | 5 | `AutoNumber`, `RecNo`, `RowNo`, `IterNo` |
| Record | 5 | `Exists`, `Peek`, `Lookup`, `Previous` |
| Math | 5 | `Pi`, `e`, `Null`, `True`, `False` |
| Window | 3 | `Window`, `WRank` |
| Mapping | 2 | `ApplyMap`, `MapSubString` |

## Supported Script Statements

`LOAD`, `SELECT`, `SQL`, `SET`, `LET`, `STORE`, `DROP TABLE/FIELD`, `RENAME TABLE/FIELD`, `TAG/UNTAG FIELD`, `QUALIFY/UNQUALIFY`, `MAPPING LOAD`, `LEFT/RIGHT/INNER/OUTER JOIN`, `LEFT/RIGHT/INNER KEEP`, `CONCATENATE`, `CROSSTABLE`, `INTERVALMATCH`, `HIERARCHY`, `SECTION ACCESS/APPLICATION`, `DIRECT QUERY`, `DECLARE`, `DERIVE`, `CONNECT TO`, `DISCONNECT`, `EXECUTE`, `BINARY`, `BUFFER`, `INCLUDE`, `TRACE`, `SLEEP`, and more.

## Supported Control Statements

`IF/THEN/ELSE/ELSEIF/END IF`, `FOR/NEXT`, `FOR EACH/NEXT`, `DO WHILE/LOOP`, `DO UNTIL/LOOP`, `SUB/END SUB`, `SWITCH/CASE/DEFAULT/END SWITCH`, `CALL`, `EXIT SCRIPT/FOR/DO`.

## Installation

1. Copy the `vscode-qlik` folder to your VS Code extensions directory:
   - **Windows**: `%USERPROFILE%\.vscode\extensions\`
   - **macOS**: `~/.vscode/extensions/`
   - **Linux**: `~/.vscode/extensions/`
2. Restart VS Code
3. Open any `.qvs` file to see syntax highlighting

## Credits

- Original extension by [Xavier Hahn (Gimly)](https://github.com/Gimly/vscode-qlik)
- Updated grammar based on Qlik Sense November 2026 SR2 BNF specification
- Maintained by [bintocher](https://github.com/bintocher)

## License

MIT
