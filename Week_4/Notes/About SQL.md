# About SQL
### *SQL Keywords*
SQL keywords are used to specify actions in your queries. SQL keywords are not case sensitive, but we suggest using all caps for SQL keywords so that you can easily set them apart from the rest of the query. Some frequently used keywords are:

**SELECT**

SELECT allows us to grab data for specific columns from the database:
* * (asterisk): it is used after SELECT to grab all columns from the table;
* column_name(s): to select specific columns, put the names of the columns after SELECT and use commas to separate them.
* 
**FROM**

FROM allows us to specify which table(s) we care about; to select multiple tables, list the table names and use commas to separate them. (But until you learn the JOIN keyword, you may be surprised at what happens.)

**WHERE**

The WHERE clause in a query is used to filter results by specific criteria.

**AND**

The AND keyword is used to string together multiple filtering criteria so that the filtered results meet each and every one of the criteria. (There’s also an OR keyword, which returns rows that match any of the criteria.)

**Wildcards and other functions for partial matches**

Sometimes you only know part of the information you need. SQL can handle that. Special symbols that represent unknown characters are called “wildcards,” and SQL supports two. The most common is the `%` wildcard.
When you place a `%` wildcard in a query string, the SQL system will return results that match the rest of the string exactly, and have anything (or nothing) where the wildcard is. For example, `’Ca%a’ `matches `Canada` and `California`.
The other, less commonly used wildcard, is` _`. This one means ‘match the rest of the text, as long as there’s exactly one character in exactly the position of the `_`, no matter what it is. So, `’B_b’` would match `’Bob’ `and `’Bub’` but not `’Babe’` or `’Bb’`.

**Important:** When using wildcards, you don’t use the `=` symbol; instead, you use `LIKE`.

SQL commands are not case-sensitive, but `WHERE` queries values for `=` and `LIKE` are. Sometimes you don’t know how the text is stored in the database. SQL provides a couple of functions which can smooth that out for you. They’re called `UPPER()` and `LOWER()`

Here are a few useful aggregate functions SQL provides:

**MAX**
finds the maximum value
**MIN**
finds the minimum value
**SUM**
calculates the sum of the specified column values
**AVG**
calculates the average of the specified column values
**COUNT**
counts the number of specified column values

There’s another way to find minimum and maximum values, while also seeing more of the data. You can control the sort order of results you get. It’s really quite intuitive: just use `ORDER BY` followed by a column name. It can be challenging when there’s a lot of data! (When people get serious about working with SQL, they use better tools than this web-based system!) By default, `ORDER BY` goes in “ascending” (smallest to largest, or A to Z) order, but you can be specific with `ASC` for ascending, or you can reverse it with `DESC`.
