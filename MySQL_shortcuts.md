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

### 