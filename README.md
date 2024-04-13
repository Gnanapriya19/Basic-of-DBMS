MANIPULATE A DATABASE BY CREATING, INSERTING, DELETING, UPDATING AND RETRIEVING TABLES 
 
AIM: 
 
To execute SQL commands for creating tables, retrieving the values, inserting, updating and deleting values from the table. 
 
PROCEDURE: 
 
1.	Creating a Database 
 
Create is a DDL SQL command used to create a table or a database in relational database management system. 
To create a database in RDBMS, create command is used.  
 
Syntax: 
 
	 	CREATE DATABASE <DB_NAME>; 
 
Example: 
 
	 	CREATE DATABASE Test; 
 
The above command will create a database named Test, which will be an empty schema without any table. 
 
 
2.	Creating a Table 
 
Create command can also be used to create tables. Now when we create a table, we have to specify the details of the columns of the tables too. We can specify the names and data types of various columns in the create command itself. 
Syntax: 
 
CREATE TABLE <TABLE_NAME> (column_name1 datatype1, column_name2 datatype2, column_name3 datatype3, column_name4 datatype4); 
 
Example: 
 
	 	CREATE TABLE Employee 
( 
    EmployeeNo char(4), 
    EmployeeName varchar2(30), 
    EmployeeSal number(10,2), 
    EmployeeCity varchar2(30), 
    EmployeeDob date 
); 
The above command will create a table named emp. 
3.INSERT SQL command 
 
Data Manipulation Language (DML) statements are used for managing data in database. DML commands are not auto-committed. It means changes made by DML command are not permanent to database, it can be rolled back. 
Syntax: 
 
 INSERT INTO table_name VALUES(data1, data2, ...) 
 
Example: 
INSERT INTO Employee(EmployeeNo, EmployeeName, EmployeeSal, EmployeeCity, EmployeeDob) Values(('1', 'Arvind', 5000, 'Mumbai','23-DEC-1992'); 
 
Other Options to insert records, using this technique all the table's columns are required. 
INSERT INTO Employee values('2', 'Santosh', 5000, 'Delhi','23-DEC-1994'); 
4.Select Command  
 
The SQL SELECT statement is used to fetch the data from a database table which returns this data in the form of a result table. These result tables are called result-sets. 
Syntax : 
 
The basic syntax of the SELECT statement is as follows − 
 
SELECT column1, column2, columnN FROM table_name; 
 
Here, column1, column2... are the fields of a table whose values you want to fetch. If you want to  fetch all the fields available in the field, then you can use the following syntax. 
 
SELECT * FROM table_name; 
Example: 
select * from Employee 
select EmployeeNo, EmployeeName, EmployeeSal,EmployeeCity,EmployeeDob from 
Employee 
5.UPDATE Command 
 
UPDATE command is used to update any record of data in a table.  
 
Syntax: 
 
UPDATE table_name SET column_name = new_value WHERE some_condition; 
 
 WHERE is used to add a condition to any SQL query. 
 
Example: 
 
UPDATE Employee SET EmployeeName='KASHISH' WHERE EmployeeNo=1 
5.DELETE Command 
 
DELETE command is used to delete data from a table.  
 
Syntax: 
 
DELETE FROM table_name; Example : 
DELETE FROM EMPLOYEE WHERE employeeNo=1 
 
         
1(a).MANIPULATE A DATABASE BY CREATING, INSERTING, DELETING, UPDATING AND RETRIEVING TABLES. 
 
COMMANDS: 
 
SQL> CREATE DATABASE Test; 
Database Created 
   SQL> CREATE TABLE Employee(EmployeeNo char(4), EmployeeName varchar2(30),         
   EmployeeSal number(10,2),   EmployeeCity varchar2(30), EmployeeDob date); 
   Table Created 
SQL> INSERT INTO Employee values('2', 'Santosh', 5000, 'Delhi','23-DEC-1994'); 
    1 row inserted 
    SQL>select * from Employee; 
	 	  
 
SQL> UPDATE Employee SET EmployeeName='KASHISH' WHERE EmployeeNo=1; SQL>SELECT * from Employee; 
	 	  
SQL>DELETE * from Employee; 
0 row(s) deleted 
 
 
 
 
RESULT: 
Thus, the SQL commands for creating tables, retrieving the values, inserting, updating and deleting values from the table is executed successfully. 


