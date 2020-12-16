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

###  