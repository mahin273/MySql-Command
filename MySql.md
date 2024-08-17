+To show all the databases available on computer
    => SHOW DATABASES;

+To select a particular database to run queries on
    => USE <database name>;

+To list down all the tables of a particular selected database
    => SHOW TABLES;

+To create a new databases
    =>CREATE DATABASE <name>;

+To create table
    => CREATE TABLE <name> (
        <column name 1> [datatype]<keyword>,
        <column name 2> [datatype],
        .
        .
    );

+To show structure and description of the table
    => DESC <table name>;

+To insert info at the table
    => INSERT INTO<table name> (col1, col2, ....) VALUES (<value1>, <value2>, .....)

+Insert Multiple Data at once
    =>INSERT INTO second (Name,DoB,Gender) 
      VALUES
     ("Mahin","2002-12-28","Male"),
     ("Tamim","2004-02-09","Male"),
     ("Abdul","2003-05-07","Male"),
     ("Riana","2001-02-01","Female");

+To get a specific column data from a table
    =>SELECT<column name> FROM <table name>;

+To get all column data from a table
    =>SELECT * FROM <table name>;

+Select data under conditon
    =>SELECT * FROM <table name> WHERE {condition..}

+Select data under multiple condition
    =>SELECT * FROM <table name> WHERE {condition..} AND {condition..} 

+Select data under any one condition
    =>SELECT * FROM <table name> WHERE {condition..} OR {condition..}  

+Search using specific keyword
    =>SELECT * FROM <table name> WHERE  {Conditonn..} LIKE ="%keyword";

+Search using specific keyword from firs t
    =>SELECT * FROM <table name> WHERE  {Conditonn..} LIKE ="_letter%";

+Select data under NOT condition
    =>SELECT * FROM <table name> WHERE NOT {condition..};

+Select data under specific order
    =>SELECT * FROM <table name> ORDER BY {column name}; //will sort in ascending order
    =>SELECT * FROM <table name> ORDER BY {column name} DESC; //will sort in decending order

+Select data using LIMIT 
    =>SELECT * FROM <table name> ORDER BY {column name} DESC LIMIT n;//Will give us n th firt row

+Select data under specific condition and using LIMIT 
    =>SELECT * FROM <table name> WHERE {condition..}ORDER BY {column name} DESC LIMIT n;

+Delete data from table
    =>DELETE FROM <TABLE NAME> WHERE{COMPARISSON..}ORDER BY .. LIMIT..;

+Delete all data from table
    =>DELETE FROM <TABLE NAME>;

+Update the data in a table
    =>UPDATE <table name> SET <column 1> = value 1 WHERE {conditions};

+Change the structure of the table
    =>ALTER TABLE <TABLE NAME> CHANGE < old column name> <new column name>[new constraint(datatype or consraint)];

+Add Column to the table
    =>ALTER<table name> ADD <column name> [parameters-data type and constains]

+Add Column to a specific position of the table
    =>ALTER TABLE <table name> ADD <column name> [parameters-data type and constains] AFTER <name of the column name which next to add>

+Delete Column  the of a table
    =>ALTER TABLE <table name> DROP <Column name>


#SELECT
--------
=>SELECT <column name> AS "Date of Birth" FROM <table name>;

=>SELECT CONCATE (Column1 name,' ' ,column2 name) AS Name FROM <Table name>;

+How to get distinct value
    =>SELECT DISTINCT <column name> FROM <table name>;

+How to count data from a column
    =>SELECT COUNT(*) FROM <table name> WHERE <column name> ='logic';

+How to Sum Column
 =>SELECT COUNT(*) AS "Name" FROM <Table name> WHERE <clumn name> =' ';

+How to get Average
=>SELECT AVG(column name) FROM<table name> WHERE <Column name> =' ';

+GROUP BY
----------
=>SELECT <Column Name>, Count(*) FROM <Table name> Group BY <Column name> ORDER BY <column name>;

=>SELECT COUNT(*) FROM <table name> GROUP BY <column name> HAVING <col name> =/>' ';

TASK-->Try to run them combined different command

#JOINS(Right, Left, Inner and Outer Joins + Self join)
======================================================= 
+Inner Join
=>SELECT * FROM <table 1> INNER JOIN <table 2> ON {Join Condition  } 
Ex:SELECT * FROM Actors INNER JOIN Assets ON Actor.Id = Assets.Id;

+Right Join
=>SELECT * FROM <table 1> RIGHT JOIN <table 2> ON {Join Condition;

+Left Join
=>SELECT * FROM <table 1> LEFT JOIN <table 2> ON {Join Condition;  

*if column name is same then we can use USING function*

