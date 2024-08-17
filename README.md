To show all the databases available on the computer, use the following command:
```
SHOW DATABASES;
```

To select a particular database to run queries on, use the following command:
```
USE <database name>;
```

To list down all the tables of a particular selected database, use the following command:
```
SHOW TABLES;
```

To create a new database, use the following command:
```
CREATE DATABASE <name>;
```

To create a table, use the following command:
```
CREATE TABLE <name> (
    <column name 1> [datatype] <keyword>,
    <column name 2> [datatype],
    ...
);
```

To show the structure and description of a table, use the following command:
```
DESC <table name>;
```

To insert information into a table, use the following command:
```
INSERT INTO <table name> (col1, col2, ...) VALUES (<value1>, <value2>, ...);
```

To insert multiple data at once, use the following command:
```
INSERT INTO second (Name, DoB, Gender) 
VALUES
("Mahin", "2002-12-28", "Male"),
("Tamim", "2004-02-09", "Male"),
("Abdul", "2003-05-07", "Male"),
("Riana", "2001-02-01", "Female");
```

To get a specific column data from a table, use the following command:
```
SELECT <column name> FROM <table name>;
```

To get all column data from a table, use the following command:
```
SELECT * FROM <table name>;
```

To select data under a condition, use the following command:
```
SELECT * FROM <table name> WHERE {condition..};
```

To select data under multiple conditions, use the following command:
```
SELECT * FROM <table name> WHERE {condition..} AND {condition..};
```

To select data under any one condition, use the following command:
```
SELECT * FROM <table name> WHERE {condition..} OR {condition..};
```

To search using a specific keyword, use the following command:
```
SELECT * FROM <table name> WHERE {condition..} LIKE "%keyword";
```

To search using a specific keyword from the first, use the following command:
```
SELECT * FROM <table name> WHERE {condition..} LIKE "_letter%";
```

To select data under a NOT condition, use the following command:
```
SELECT * FROM <table name> WHERE NOT {condition..};
```

To select data under a specific order, use the following command:
```
SELECT * FROM <table name> ORDER BY {column name}; // will sort in ascending order
SELECT * FROM <table name> ORDER BY {column name} DESC; // will sort in descending order
```

To select data using LIMIT, use the following command:
```
SELECT * FROM <table name> ORDER BY {column name} DESC LIMIT n; // will give us the nth first row
```

To select data under a specific condition and using LIMIT, use the following command:
```
SELECT * FROM <table name> WHERE {condition..} ORDER BY {column name} DESC LIMIT n;
```

To delete data from a table, use the following command:
```
DELETE FROM <TABLE NAME> WHERE {COMPARISON..} ORDER BY .. LIMIT..;
```

To delete all data from a table, use the following command:
```
DELETE FROM <TABLE NAME>;
```

To update the data in a table, use the following command:
```
UPDATE <table name> SET <column 1> = value 1 WHERE {conditions};
```

To change the structure of a table, use the following command:
```
ALTER TABLE <TABLE NAME> CHANGE <old column name> <new column name> [new constraint(datatype or constraint)];
```

To add a column to a table, use the following command:
```
ALTER TABLE <table name> ADD <column name> [parameters-data type and constraints];
```

To add a column to a specific position of a table, use the following command:
```
ALTER TABLE <table name> ADD <column name> [parameters-data type and constraints] AFTER <name of the column name which is next to add>;
```

To delete a column of a table, use the following command:
```
ALTER TABLE <table name> DROP <Column name>;
```

To select a column with an alias, use the following command:
```
SELECT <column name> AS "Date of Birth" FROM <table name>;
```

To concatenate column values, use the following command:
```
SELECT CONCAT(Column1 name, ' ', column2 name) AS Name FROM <Table name>;
```

To get distinct values, use the following command:
```
SELECT DISTINCT <column name> FROM <table name>;
```

To count data from a column, use the following command:
```
SELECT COUNT(*) FROM <table name> WHERE <column name> = 'logic';
```

To sum a column, use the following command:
```
SELECT COUNT(*) AS "Name" FROM <Table name> WHERE <column name> = ' ';
```

To get the average, use the following command:
```
SELECT AVG(column name) FROM <table name> WHERE <Column name> = ' ';
```

To group by a column, use the following command:
```
SELECT <Column Name>, Count(*) FROM <Table name> GROUP BY <Column name> ORDER BY <column name>;
```

For joins (Right, Left, Inner, and Outer Joins + Self join), use the following commands:
```
Inner Join:
SELECT * FROM <table 1> INNER JOIN <table 2> ON {Join Condition};

Right Join:
SELECT * FROM <table 1> RIGHT JOIN <table 2> ON {Join Condition};

Left Join:
SELECT * FROM <table 1> LEFT JOIN <table 2> ON {Join Condition};
```

If the column names are the same, you can use the USING function.

Remember to replace `<database name>`, `<name>`, `<column name>`, `<table name>`, `<value1>`, `<value2>`, `{condition..}`, `{COMPARISON..}`, `{column name}`, `n`, `<old column name>`, `<new column name>`, `<column name 1>`, `<column name 2>`, `<keyword>`, `<Table name>`, `<Column Name>`, `<Column1 name>`, `<column2 name>`, `logic`, `_letter`, `keyword`, and `<Join Condition>` with the appropriate values and conditions.
