
Types of SQL Commands
```
Data Definition Language / DDL: It's used to construct and modify the structure of database objects in the database. Commands are: CREATE, DROP, ALTER, TRUNCATE

Data Manipulation Language / DML: It's deal with manipulating data in a database are classified, which covers the majority of SQL statements. Commands are: INSERT, UPDATE, DELETE

Data Control Language / DCL: It's a query language that allows users to retrieve and edit data held in databases. Commands are: GRANT, REVOKE

Transaction Control Language / TCL: These instructions are used in the database to manage transactions. Commands are: COMMIT, ROLLBACK, SAVEPOINT

Data Query Language / DQL: these statements are used to query the data contained in schema objects. Commands are: SELECT
```

Some of The Most Important SQL Commands
```
SELECT:  Extracts data from a database
UPDATE:  Updates data in a database
DELETE:  Deletes data from a database
INSERT INTO:  Inserts new data into a database
CREATE DATABASE:  Creates a new database
ALTER DATABASE:  Modifies a database
CREATE TABLE:  Creates a new table
ALTER TABLE:  Modifies a table
DROP TABLE:  Deletes a table
CREATE INDEX:  Creates an index (search key)
DROP INDEX:  Deletes an index
```

`SELECT` Statement
```
Syntax:
SELECT column1, column2, ...
FROM database_name;

Example:
SELECT Username, MobileNumber, Email FROM Users;
```

`SELECT DISTINCT` Statement
```
Syntax:
SELECT DISTINCT column1, column2, ...
FROM table_name;

Example:
SELECT DISTINCT Country FROM Users;
SELECT DISTINCT Country, City FROM Users;
```

`WHERE` Statement
```
Syntax:
SELECT column1, column2, ...
FROM table_name
WHERE condition;

Operators:
=          Equal
>          Greater than
<          Less than
>=         Greater than or equal
<=         Less than or equal
<>         Not equal
BETWEEN    Between a certain range
LIKE       Search for a pattern
IN         To specify multiple possible values for a column

Example:
SELECT * FROM Users WHERE 1;
SELECT * FROM Users WHERE UserId >= 3;
SELECT * FROM Users WHERE IsSubscribed = 1;
SELECT * FROM Users WHERE Country <> 'United States';
SELECT * FROM Users WHERE City IN ('Yerevan', 'Paris', 'Stockholm');
```

`ORDER BY` Keyword
```
Syntax:
SELECT column1, column2, ....
FROM table_name
ORDER BY column1, column2, ... ASC|DESC;

Example:
SELECT * FROM Users ORDER BY NationalCode;
SELECT * FROM Users ORDER BY NationalCode DESC;
SELECT * FROM Users ORDER BY NationalCode, Country DESC;
SELECT * FROM Users ORDER BY NationalCode ASC, Country DESC;
```

`AND`, `OR` Operator:
```
Syntax:
SELECT column1, column2, ...
FROM table_name
WHERE condition1 AND condition2 AND condition3 AND ...;

Example:
SELECT * FROM Users WHERE Country <> 'United States' AND IsSubscribed = 1;
SELECT * FROM Users WHERE Email LIKE '%@gmail.com' AND (Country = 'Iran' OR Country = 'United States');
SELECT * FROM Users WHERE Email IS NOT NULL AND IsSubscribed = 1;
```

