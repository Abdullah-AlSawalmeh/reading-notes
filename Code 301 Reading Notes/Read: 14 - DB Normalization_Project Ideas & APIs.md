## DB Normalization

1. It is a process used to organize a database into tables and columns. Take a spreadsheet containing the information as an example, where the data contains salespeople and customers serving several purposes:

   - Identify salespeople in your organization
   - List all customers your company calls upon to sell a product
   - Identify which salespeople call on specific customers.

2. reasons to normalize a database:

   - minimize duplicate data
   - minimize or avoid data modification issues
   - simplify queries

3. Duplicated information presents two problems:

   - It increases storage and decrease performance.
   - It becomes more difficult to maintain data changes.

4. Search and Sort Issues

```
SELECT SalesOffice
FROM SalesStaff
WHERE Customer1 = ‘Ford’ OR
      Customer2 = ‘Ford’ OR
      Customer3 = ‘Ford’
```

5. various forms:
   - First Normal Form – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.
   - Second Normal Form – The table is in first normal form and all the columns depend on the table’s primary key.
   - Third Normal Form – the table is in second normal form and all of its columns are not transitively dependent on the primary key
