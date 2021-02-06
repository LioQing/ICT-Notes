# SQL Summary

## Content

* [Notice](#Notice)
* [Operators](#Operators)
    - [Arithmetic Operator](#Arithmetic-Operator)
    - [Bitwise Operators](#Bitwise-Operators)
    - [Comparison Operators](#Comparison-Operators)
    - [Logic Operators](#Logic-Operators)
    - [Wildcards](#Wildcards)
        + [LIKE](#LIKE)
* [Functions](#Functions)
    - [Aggregate Function ](#Aggregate-Function)
    - [Arithmetic Function](#Arithmetic-Function)
    - [String Function](#String-Function)
* [Keyword](#Keyword)

## Notice 

This page **only** consisted all the SQL commands given in the formula sheet in **Compulsory Part** but **NOT** all the SQL commands in **Modula 2A**. \
Due to lack of information of the keyword `AT` and `BY` , the description of keyword `AT` and `BY` is **NOT** being covered in this page.\
Furthermore, `SELECT` , `FROM` , `WHERE` , `ORDER BY` and `GROUP BY` have been mentioned in [Information_Processing.md](Information_Processing.md#structured-query-language-sql-in-dbms), so it will **NOT** cover again in this page.

## Operators

### Arithmetic Operator

| Operator            |  Description   | Notes |
|---------------------|:--------------:|-------|
| `+` (Plus sign)     |    Addition    | NULL  |
| `-` (Minus sign)    |  Subtraction   | NULL  |
| `*` (Asterisk)      | Multiplication | NULL  |
| `/` (Forward slash) |    Division    | NULL  |
| `%` (percent sign)  |    Modulus     | NULL  |

### Bitwise Operators

| Operator        | Description | Notes                  |
|-----------------|:-----------:|------------------------|
| `&` (Ampersand) | Bitwise AND | **Not Given in HKDSE** |
| `\|` (Pipe)     | Bitwise OR  | **Not Given in HKDSE** |
| `~` (Tilde)     | Bitwise NOT | **Not Given in HKDSE** |

**Notes**\
If you don't know what is [Bitwise AND](https://en.wikipedia.org/wiki/Bitwise_operation#AND), [Bitwise OR](https://en.wikipedia.org/wiki/Bitwise_operation#OR) and [Bitwise NOT](https://en.wikipedia.org/wiki/Bitwise_operation#NOT) you may refer to the above links.

### Comparison Operators

Usually use in `condition(s)`

| Operator |       Description        | Notes |
|----------|:------------------------:|-------|
| =        |         Equal to         | NULL  |
| >        |       Greater than       | NULL  |
| <        |        Less than         | NULL  |
| >=       | Greater than or equal to | NULL  |
| <=       |  Less than or equal to   | NULL  |
| <>       |       Not equal to       | NULL  |

### Logic Operators

Usually use in `condition(s)`

| Operator |                      Description                      | Notes                                                                                                |
|----------|:-----------------------------------------------------:|------------------------------------------------------------------------------------------------------|
| `AND`    |  TRUE if all the conditions separated by AND is TRUE  | NULL                                                                                                 |
| `OR`     | TRUE if any of the conditions separated by OR is TRUE | NULL                                                                                                 |
| `NOT`    |   Displays a record if the condition(s) is NOT TRUE   | NULL                                                                                                 |
| `LIKE`   |         TRUE if the operand matches a pattern         | **It is given in HKDSE but NOT under the column `Operators`** <br> Syntax of `LIKE` will cover below |

### Wildcards
Before talk about `LIKE` operator, you have to know about wildcard character\
| Symbol             | Description                    | Notes                                                                           |
|--------------------|--------------------------------|---------------------------------------------------------------------------------|
| `%` (percent sign) | Matches one or more characters | MS Access uses `*` (asterisk)  wildcard character instead of `%` (percent sign) |
| `_` (underscore)   | Matches one character          | MS Access uses `?` (question mark) instead of `_` (underscore)                  |

#### LIKE
|                                                                                                                                                                                                                                 Syntax                                                                                                                                                                                                                                  |
|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| `SELECT {Column_Name} FROM{Table_Name} WHERE {Column_Name} LIKE 'XXXX%'` <br> OR <br> `SELECT {Column_Name} FROM{Table_Name} WHERE {Column_Name} LIKE '%XXXX%'` <br> OR <br> `SELECT {Column_Name} FROM{Table_Name} WHERE {Column_Name} LIKE 'XXXX_'` <br> OR <br> `SELECT {Column_Name} FROM{Table_Name} WHERE {Column_Name} LIKE '_XXXX'` <br> OR <br> `SELECT {Column_Name} FROM{Table_Name} WHERE {Column_Name} LIKE '_XXXX_'`  <br> or combinations of `%` and `_` |
## Functions

### Aggregate Function 

| Function | Description                                           | Syntax                                                             | Notes                                        |
|----------|-------------------------------------------------------|--------------------------------------------------------------------|----------------------------------------------|
| `MIN`    | Returns the smallest value of the selected column     | `SELECT MIN({Column_Name}) FROM {Table_Name} WHERE {condition};`   | **CANNOT** use directly with `WHERE` keyword |
| `MAX`    | Returns the largest value of the selected column      | `SELECT MAX({Column_Name}) FROM {Table_Name} WHERE {condition};`   | **CANNOT** use directly with `WHERE` keyword |
| `COUNT`  | Returns the number of rows that matches the condition | `SELECT COUNT({Column_Name}) FROM {Table_Name} WHERE {condition};` | **CANNOT** use directly with `WHERE` keyword |
| `AVG`    | Returns the average value of a **numeric** column     | `SELECT AVG({Column_Name}) FROM {Table_Name} WHERE {condition};`   | **CANNOT** use directly with `WHERE` keyword |
| `SUM`    | Returns the total sum of a **numeric** column         | `SELECT SUM({Column_Name}) FROM {Table_Name} WHERE {condition};`   | **CANNOT** use directly with `WHERE` keyword |

### Arithmetic Function

| Function        | Description                           | Syntax           | Notes                                                                                          |
|-----------------|---------------------------------------|------------------|------------------------------------------------------------------------------------------------|
| `ABSOLUTE(ABS)` | Return the absolute value of a number | `ABS({Numeric})` | NULL                                                                                           |
| `INT`           | Returns the integer part of a number  | `INT({Numeric})` | The function returns the first negative integer less than or equal to number if it is negative |

### String Function

| Function                 | Description                                                  | Syntax                                                                                  | Notes                                                                                                |
|--------------------------|--------------------------------------------------------------|-----------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|
| `CHAR_LENGTH (LEN)`      | Returns the length of a string (in characters)               | `CHAR_LENGTH(String)`                                                                   | NULL                                                                                                 |
| `LOWER`                  | Converts a string to lower-case                              | `LOWER(String)`                                                                         | NULL                                                                                                 |
| `UPPER`                  | Converts a string to upper-case                              | `UPPER(String)`                                                                         | NULL                                                                                                 |
| `SPACE`                  | Returns a string of the specified number of space characters | `SPACE(Number)`                                                                         | E.g. `SPACE(5)` it will create a string with 5 spaces                                                |
| `SUBSTRING (SUBSTR/MID)` | Extracts a substring from a string                           | `SUBSTRING(String, start, length)` <br>OR<br> `SUBSTRING(String FROM start FOR length)` | `MID` and `SUBSTR` same as `SUBSTRING` <br> Start position is 1-based<br> `FOR` keyword is not given |
| `TRIM`                   | Removes leading and trailing spaces from a string            | `TRIM(String)`                                                                          | It also work with numbers, for numbers it will remove the leading zeros                              |

## Keyword

| Keyword    | Description                                                                                           | Syntax                                                                                                                                             | Notes                                                                                                                                                              |
|------------|-------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `AS`       | Renames a column or table with an alias                                                               | `SELECT {Column_Name} AS {The_Name_You_Makeup} FROM {Table_Name};` <br> OR <br> `SELECT {Column_Name} FROM {Table_Name} AS {The_Name_You_Makeup};` | Usually using `AS` with `{Table_Name}` is having more than one table                                                                                               |
| `BETWEEN`  | Selects values within a given range                                                                   | `SELECT {Column_Name} FROM {Table_Name} WHERE BETWEEN {Range}`                                                                                     | NULL                                                                                                                                                               |
| `ASC`      | Sorts the result set in ascending order                                                               | `SELECT {Column_Name} FROM {Table_Name} ORDER BY {Column_Name} ASC;`                                                                               | The `ASC` only affect the column in front it. <br> E.g. `SELECT * FROM Table ORDER BY Column1, Column2 ASC;` <br> In above case only `Column2` is sorted ascending |
| `DESC`     | Sorts the result set in descending order                                                              | `SELECT {Column_Name} FROM {Table_Name} ORDER BY {Column_Name} DESC;`                                                                              | Same as `ASC` , please refer the notes above                                                                                                                       |
| `DISTINCT` | Selects only distinct values                                                                          | `SELECT DISTINCT {Column_Name} FROM {Table_Name};`                                                                                                 | NULL                                                                                                                                                               |
| `HAVING`   | To replace `WHERE` with aggregate function since `WHERE` could not be used with aggregate functions   | `SELECT {Column_Name} FROM {Table_Name} WHERE {condition} GROUP BY {Column_Name} HAVING aggregate_function({Column_Name});`                        | There are some other form of syntax, you may refer [this](https://www.w3schools.com/sql/sql_having.asp)                                                            |
| `NULL`     | A field with a `NULL` value is a field empty <br> `NULL` can be use to test weather the field is NULL | `SELECT {Column_Name} FROM {Table_Name} WHERE {Column_Name} IS NULL;`                                                                              | `IS NOT NULL` can test weather it have any value in the field                                                                                                      |
