# SQL Cheatsheet

## Unique Features
- Declarative language for managing relational databases
- Used to create, modify, and query databases
- Supports ACID transactions for data consistency
- Standardized language with multiple dialects

## Data Types
- Integer: `INT`
- Decimal: `DECIMAL`
- Character: `CHAR`
- Varying character: `VARCHAR`
- Date: `DATE`
- Time: `TIME`
- Timestamp: `TIMESTAMP`
- Boolean: `BOOLEAN`

## Creating Tables
```sql
CREATE TABLE [table name] (
   [column name] [data type] [optional parameters],
   [column name] [data type] [optional parameters],
   ...
);
```

## Inserting Data
```sql
INSERT INTO [table name] ([column name], [column name], ...) 
VALUES ([value], [value], ...);
```

## Updating Data
```sql
UPDATE [table name] 
SET [column name] = [new value], [column name] = [new value], ... 
WHERE [condition];
```

## Deleting Data
```sql
DELETE FROM [table name] WHERE [condition];
```

## Querying Data
```sql
SELECT [column name], [column name], ... 
FROM [table name] 
WHERE [condition] 
ORDER BY [column name] [ASC/DESC];
```

## Joins
```sql
SELECT [column name], [column name], ... 
FROM [table name 1] 
JOIN [table name 2] 
ON [table name 1].[column name] = [table name 2].[column name];
```

## Aggregation
```sql
SELECT COUNT([column name]) 
FROM [table name];

SELECT AVG([column name]) 
FROM [table name];

SELECT SUM([column name]) 
FROM [table name];
```

## Functions
```sql
MAX([column name])

MIN([column name])

UPPER([string])

LOWER([string])

SUBSTR([string], [start], [length])
```

## Resources
- [SQL Tutorial](https://www.w3schools.com/sql/)
- [PostgreSQL Documentation](https://www.postgresql.org/docs/)
- [MySQL Documentation](https://dev.mysql.com/doc/)