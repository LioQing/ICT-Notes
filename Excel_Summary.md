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
| RAND     | Generates a random decimal within the range 0<=x<1.| =RAND() | To scale the number to between 0 to *x*, use = x * RAND(). To scake the number to between *y* and *z*, use = (z - y) * RAND() + y
| IF       | Returns *a* if the condition given is true, *b* otherwise.| =IF(Condition,a,b) | 
| AND      | Returns true if all the conditions given are true, false otherwise.| =AND(Condition_1,Condition_2,...)| More than 2 conditions can be added.
| OR       | Returns true if any condition given is true, false otherwise.| =OR(Condition_1,Condition_2,...)| More than 2 conditions can be added.
| NOT      | Returns false if the condition given is true, false otherwise.| =NOT(Condition) |
| CODE     | Returns the ASCII key code of the first character in a string.| =CODE(String) |
| CHAR     | Returns the ASCII character as specified by the key code given.| =CHAR(Number) |
| LEN      | Returns the length (number of characters) of a string.| =LEN(String)
| LEFT     | Returns the leftmost *n* characters in the string provided.| =LEFT(String,n) | =LEFT("I IS MR WONG",3) = "I I"
| MID      | Returns a *n* characters from the string given, starting from the *p*th character.| =MID(String,n,p)| =MID("I IS MR WONG",3,4) = "IS M"
| RIGHT    | Returns the rightmost *n* characters in the string provided.| =RIGHT(String,n) | =RIGHT("I IS MR WONG",3) = "ONG"
| TEXT     | Returns the textual representation of the number given.| =TEXT(Number) | =TEXT(133)= "133"
| VALUE    | Returns the numerical representation of a piece of text.| =VALUE(String)| =VALUE("133") = 133
| DAY      | Returns the day of the Date given.| =DAY(Date) | =DAY(31/12/2077) = 31
| MONTH    | Returns the month of the Date given.| =MONTH(Date) | =MONTH(31/12/2077) = 12
| YEAR     | Returns the year of the Date given.| =YEAR(Date) | =YEAR(31/12/2077) = 2077
| WEEKDAY  | Finds the day of the week of this Date, in a numeric form.| =WEEKDAY(Date) | 1 = Sunday, 2 = Monday, 3 = Tuesday, ..., 7 = Saturday (=WEEKDAY(6/1/2021) = 4)
| TODAY    | Finds the current day. | =TODAY() | 
| HLOOKUP  | Looks up data according to a given value. | =HLOOKUP(Exact, Range, p, Exact)| Horizontally looks for the value *n* in the first row of the range given. If *Exact* is false, a comparison is used to find the most matching data. Otherwise, only equal results will count as a success. When the value is found, looks *p* cells down for the value to return.
| VLOOKUP  | Looks up data according to a given value. | =VLOOKUP(Exact, Range, p, Exact)| Vertically looks for the value *n* in the first row of the range given. If *Exact* is false, a comparison is used to find the most matching data. Otherwise, only equal results will count as a success. When the value is found, looks *p* cells to the right for the value to return.
