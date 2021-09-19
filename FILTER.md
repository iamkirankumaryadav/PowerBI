# FILTER

- Returns a `Table` that represents a subset of another table or expression.
- Add a new `Filter Context`
- `FILTER` is a `CALCULATE` Modifier and a `Iterator` function.

```DAX
FILTER ( Table, Expression )
```

`Table` : `Lookup` or `Dimension` Table 

Calender[Year] = 2021, Sales[Price] > [Avg Price] )

`Expression` : Boolean Expression that creates a subset of table or a calculated `Measure` 

Example 

```DAX
India Sales = 
CALCULATE (
    [Total Sales],                          
    FILTER ( 
        Region,                     // Table
        Region[Country] = "India"   // Expression (Boolean)
    )
)
```

Because `FILTER` returns a `Table`, it can be used as a input to an another function.
