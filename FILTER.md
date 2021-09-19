# FILTER

- Returns a `Table` that represents a subset of another table or expression.
- Add a new `Filter Context`

FILTER ( Table, Expression )

`Table` : `Lookup` or `Dimension` Table ( e.g. Calender[Year] = 2021, Sales[Price] > [Avg Price] )

`Expression` : Boolean Expression that creates a subset of table or a calculated `Measure` 
