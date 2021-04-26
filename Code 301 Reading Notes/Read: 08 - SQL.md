## SQL

### Introduction to SQL

1. What is SQL?

   - SQL, or Structured Query Language, is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database. And due to its simplicity, SQL databases provide safe and scalable storage for millions of websites and mobile applications.

2. Relational databases
   - A relational database represents a collection of related (two-dimensional) tables. Each of the tables are similar to an Excel spreadsheet, with a fixed number of named columns (the attributes or properties of the table) and any number of rows of data.

### Lesson 1. SELECT queries 101

```
Select query for a specific columns
SELECT column, another_column, …
FROM mytable;
```

```
Select query for all columns
SELECT *
FROM mytable;
```

### Lesson 2: Queries with constraints

```
Select query with constraints
SELECT column, another_column, …
FROM mytable
WHERE condition
    AND/OR another_condition
    AND/OR …;
```

- Standard numerical operators: =, !=, < <=, >, >=
- Number is within range of two values (inclusive): BETWEEN … AND …
- Number is not within range of two values (inclusive): NOT BETWEEN … AND
- Number does not exist in a list: NOT IN (…)
- Number exists in a list: IN (…)

### Lesson 3: Queries with constraints

- Case sensitive exact string comparison (notice the single equals): =
- Case sensitive exact string inequality comparison: != or <>
- Case insensitive exact string comparison: LIKE
- Case insensitive exact string inequality comparison: NOT LIKE
- Used anywhere in a string to match a sequence of zero or more characters (only with LIKE or NOT LIKE): %
- Used anywhere in a string to match a single character (only with LIKE or NOT LIKE): \_
- String exists in a list: IN (…)
- String does not exist in a list: NOT IN (…)

### Lesson 4: Filtering and sorting Query results

```
Select query with unique results
SELECT DISTINCT column, another_column, …
FROM mytable
WHERE condition(s);
```

```
Select query with ordered results
SELECT column, another_column, …
FROM mytable
WHERE condition(s)
ORDER BY column ASC/DESC;
```

```
Select query with limited rows
SELECT column, another_column, …
FROM mytable
WHERE condition(s)
ORDER BY column ASC/DESC
LIMIT num_limit OFFSET num_offset;
```

### Lesson 13: Inserting rows

1. Lesson 13: Inserting rows

   - what describes the structure of each table, and the datatypes that each column of the table can contain.

2. Inserting new data

   - When inserting data into a database, we need to use an INSERT statement, which declares which table to write into, the columns of data that we are filling, and one or more rows of data to insert.

   ````
   Insert statement with values for all columns
   INSERT INTO mytable
   VALUES (value_or_expr, another_value_or_expr, …),
       (value_or_expr_2, another_value_or_expr_2, …),
       …;
    ```
   ````

### Lesson 14: Updating rows

```
Update statement with values
UPDATE mytable
SET column = value_or_expr,
    other_column = another_value_or_expr,
    …
WHERE condition;
```

### Lesson 15: Deleting rows

```
Delete statement with condition
DELETE FROM mytable
WHERE condition;
```

### Lesson 16: Creating tables

```
Create table statement w/ optional table constraint and default value
CREATE TABLE IF NOT EXISTS mytable (
    column DataType TableConstraint DEFAULT default_value,
    another_column DataType TableConstraint DEFAULT default_value,
    …
);
```

1. Table data types

   - INTEGER, BOOLEAN
   - FLOAT, DOUBLE, REAL
   - CHARACTER(num_chars), VARCHAR(num_chars), TEXT
   - DATE, DATETIME
   - BLOB

2. Table constraints
   - PRIMARY KEY
   - AUTOINCREMENT
   - UNIQUE
   - NOT NULL
   - CHECK (expression)
   - FOREIGN KEY

```
Movies table schema
CREATE TABLE movies (
    id INTEGER PRIMARY KEY,
    title TEXT,
    director TEXT,
    year INTEGER,
    length_minutes INTEGER
);
```

### Lesson 17: Altering tables

1. Adding columns

```
Altering table to add new column(s)
ALTER TABLE mytable
ADD column DataType OptionalTableConstraint
    DEFAULT default_value;
```

2. Removing columns

```
Altering table to remove column(s)
ALTER TABLE mytable
DROP column_to_be_deleted;
```

3. Renaming the table

```
Altering table name
ALTER TABLE mytable
RENAME TO new_table_name;
```

### Lesson 18: Dropping tables

```
Drop table statement
DROP TABLE IF EXISTS mytable;
```
