# Discovering Data

## Week 1

[SQL introduction](#sql-introduction)  
[Like operator](#like-operator)  
[Insert Update Delete](#insert-update-delete)  
[Date and Time functionalities](#date-and-time-functionalities)

### SQL introduction

SQL means Structured Query Language and is used for querying a database. To select a column or multiple columns from a table you can use:

```sql
SELECT column1, column2 
FROM table;
```

If you want to query all columns from a table, you can use a * :

```sql
SELECT * 
FROM table;
```

To rename a column in your query, you can use the keyword AS:

```sql
SELECT column1 AS name 
FROM table;
```
To eliminate double values in your query result, you can use the keyword DISTINCT:

```sql
SELECT DISTINCT column1 
FROM table;
```
And if you would like to sort the query result, you can use ORDER BY. The suffix ASC or DESC indicates whether someting should be sorted in ascending or descending order. If no suffix is used, the default is ASC. Per column you can determine how you would like to sort it:

```sql
SELECT column1, column2
FROM table
ORDER BY column2 DESC;
```
In the next example, the query result is sorted descending on column2 first and then ascending on column3.

```sql
SELECT column1, column2, column3
FROM table
ORDER BY column2 DESC, column3;
```

After the WHERE keyword within a query, you can add (multiple) conditions. It is used to filter data from your query result:

```sql
SELECT column1, column2
FROM table
WHERE ...
```
If you only want data, where a column has a specific value, you can use:

```sql
SELECT column1, column2
FROM table
WHERE column2 = 'specific value';
```
The comparison operators you can use in the WHERE clause are:

|operator|description|
|---|---|
|<| less than|
|>| greater than|
|<=| less than or equal to|
|>=| greater than or equal to|
|=| equal|
|<> or !=| not equal|

More filters in the where clause can be combined with the keyword AND or OR:

```sql
SELECT column1, column2, column3
FROM table
WHERE ...
AND ...
```
The number of results can be limited with the keyword LIMIT, followed by a number:

```sql
SELECT column1, column2
FROM table
LIMIT ...
```

Summarized:

```sql
SELECT column1, column2
FROM table
WHERE ...
AND ...
ORDER BY column2
LIMIT ...
```

### Like operator

### Insert Update Delete

### Date and Time functionalities
