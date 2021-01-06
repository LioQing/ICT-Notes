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
| ROUND    | Rounds the value *n* to the specified number *p* of decimal places. | =ROUND(n,p) |
| INT      | Rounds down (casts) the value given to an integer.| =INT(Number) |
| MOD      | Finds the remainder (mod) of the division between number *n* and dividend *p*.| =MOD(n,p)| =MOD(9,2) = 1
| POWER    | Returns the value of the base *n* to the power *p*.| =POWER(N,P)| =POWER(3,2, = 9
| RAND     | Generates a random decimal within the range 0<=x<1.| =RAND() | To scale the number to between 0 to *x*, use = *x* * RAND(). To scake the number to between *y* and *z*, use = (*z* - *y*) * RAND() + *y*
|
