# Excel Summary Table

| Function | Description | Formula | Explanation/Note
|----------|-------------|---------|------------
| MAX      | Finds the maximum value of a range of cells.| =MAX(Range) | 
| MIN      | Finds the minimum value of a range of cells.| =MIN(Range) | 
| AVERAGE  | Finds the average numerical value of a range of cells.| =AVERAGE(Range) | 
| COUNT    | Finds the number of cells containing numerical data.| =COUNT(Range) | 
| COUNTIF  | Counts the number of cells which contain data fulfilling a specific condition.| =COUNTIF(Range,Condition) | 
| LARGE    | Finds the *n*th largest value within the given range of cells.| =LARGE(Range,n) | =LARGE(Range,1) is equal to =MAX(Range)
| SMALL    | Finds the *n*th smallest value within the given range of cells.| =SMALL(Range,n) | =SMALL(Range,1) is equal to =MIN(Range)
| MODE     | Finds the mode of the set of data given.| =MODE(RANGE) | 
| SUM      | Finds the sum of the numeric data in the range given.| =SUM(Range) |
| SUMIF    | Finds the sum of the values within the *sum range* if the corresponding entries in the *cell range* fit the condition given. | =SUMIF(Range (Cell),Condition, Range (Sum)) | The formula looks up each cell in the *cell range* consecutively, then applies *condition* to it. If *condition* return true, the corresponding value in the *sum range* is added to the current total. The total is then the result of the formula.
|
|
|
|
|
|
