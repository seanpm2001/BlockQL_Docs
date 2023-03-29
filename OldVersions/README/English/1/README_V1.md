
***

# BlockQL Docs

Currently just a modified copy of the main project `README` as there isn't much to it yet.

## Queries

Queries can be written in:

- C
- CodeQL
- D
- Java
- Python
- R
- Rust
- VBA
- More languages coming soon

## Spreadsheets

Spreadsheets can also be imported in the following formats:

- `*.dbf`
- `*.dif`
- `*.fods`
- `*.ods`
- `*.ots`
- `*.slk`
- `*.uos`
- `*.xlsx`
- `*.xls`
- More formats coming soon

## File format

BlockQL has 2 file formats:

- `*.bloql` (project file, shortened form of BlockQL, official pronunciation is block L)
- `*.bloqs` (spreadsheet file, official pronunciation is blocks)

## Syntax

### Hello World

```rust
"Hello World"
```

### Basic query

```sql
-- DEF Coin = integer(250)
import shop
usr: "ANNA" has "Banana"
usr: "ABBY" has "Coin{12}"
usr: "SHOP" has "Banana{tc:250{Coin}}"
-- tc: Total cost
join "ABBY","SHOP"
return "SHOP" getResponse "Purchase"
-- Should return:
"SHOP: User ABBY cannot buy the banana, ABBY needs 238 more coins"
```

> **Note** `shop` is a demo library that has not yet been created.

### Comments

```brainfuck
-- Single line comment
-=-
Block Comment
-=-
````

Needs more planning, language might be rewritten.

***

**File version:** `1 (2023, Tuesday, March 28th at 7:43 pm PST)`

***
