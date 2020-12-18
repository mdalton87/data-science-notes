# Important SQL Syntax and Commands
## **Databases**
### One Column
- SELECT database_column FROM database_name.table_name


### Multiple columns
- SELECT column1, column2 FROM database_name.table_name
- "*" = **ALL** columns 

### Literally shows all databases
- show databases;

### set "current working database"
- USE fruits_db;

### Show the currently selected database (kind of like pwd in GIT)
- select database();

### Show code that created this DB
- show create database fruits_db; 

## **Tables**

###  Creating a table
- CREATE TABLE table_name (
    column1_name data_type,
    column2_name data_type,
    ...
);

- Example 1:
    - CREATE TABLE quotes (
    author_first_name VARCHAR(50),
    author_last_name  VARCHAR(100) NOT NULL,
    content TEXT NOT NULL
    );

- Example 2:
     - CREATE TABLE quotes (
    id INT UNSIGNED NOT NULL AUTO_INCREMENT,
    author_first_name VARCHAR(50),
    author_last_name  VARCHAR(100) NOT NULL,
    content TEXT NOT NULL,
    PRIMARY KEY (id)
    );
        - AUTO_INCREMENT
            - instructs MySQL to generate a new values for this column
        - PRIMARY KET (id)
            - specifies that the PRIMARY KEY for the table is id

## **Basic Statements**
### Where puts a condition to limit the return 
 - SELECT column1, column2, ...
FROM table_name
WHERE column_name = 'value';
### Between, it's pretty obvious how this is used...
- SELECT column1, column2, ...
FROM table_name
WHERE column_name BETWEEN 'value1' AND 'value2';
- SELECT can be used similarly to the "print" function in python (not common)
## **Where operator**
### format is column operator value
### like first_name = 'Georgi'
- select * from employees where first_name = 'Georgi';
- select * from salaries where salary < 50000;
- select * from employees where emp_no between 20000 and 20050;
- select * from employees where hire_date between '1991-01-01' and '1992-01-01';

### Show me everybody except all the Georgis
- select * 
from employees
where first_name != 'Georgi';


### Compare the following two queries. Pay attention to the column name in the output.
- select concat(first_name, " ", last_name) 
from employees;

- select concat(first_name, " ", last_name) as full_name
from employees;

### The following two queries run identically. The new line characters don not impact performance.
- select * from employees where first_name = 'Georgi';

- select * 
from employees
where first_name = 'Georgi';

### Notice that we can add logical operators like or/and between the column = value part of the WHERE clause.
- select *
from employees
where first_name = 'Georgi'
or first_name = 'Mary';



## **Order By operator**
- Just sorts a column, ASC or DESC
### How to sort (we  will cover this more deeply very soon)
= select *
from employees
where first_name = 'Georgi'
or first_name = 'Mary'
order by first_name;













