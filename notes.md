# SQL

## 12/16/2020

## Vocabulary 

- **RDBMS:** The software that manages the data, i.e. handles it's storage and retrieval. Runs the database server
- **Database:** Sometimes used interchangably with a DBMS; The actual location of the data stored on disk; You won't interact with this directly, but rather, through the DBMS.
- **Database Client:** a program that can be used to connect to a database. Each database usually comes with an officially sanctioned command line client, and there are many different GUI database clients as well.
- **Database Server:** a computer that runs the DBMS and stores the data, typically either on-premises or in the cloud.
- **DDL:** Data definition language; commands that change the structure of the database or the DBMS itself, or change the structure of tables in the database. We will not be focusing on this part of SQL.
- **DML:** Data manipulation language; used to insert, ***update, delete, and retrieve*** information from databases. We will be focusing on the the retrieval part of this.
- **SQL** = Structured Query Language

### **Databases store information**
-  better than your file system
- contain 10 million rows (records) of info
- better optimized for storage and space than a .csv

### **Queries**



### **Databases**
SCHEMA = DATABASE in **MySQL**

MySQL server responds with NULL as the database name, most likely you do not have any database selected


### **Tables**
- like spreadsheets, but more more strict

- **Data types**
    - Numeric types
        - int, 
        - float, 
        - decimal(length, precision)
            - set number of decimal places (money)
    - Unsigned
        - only positive numbers
    - Boolean
        - MySQL has no native support for boolean values
        - TINYINT data type that goes from -128 to 127 and treats 0 as false and 1 as true
    - String types
        - CHAR(length)
            - limit number a characters (less memory) e.g. zip-code, phone numbers, etc
            - 1 - 255
        - VARCHAR(length)
            - 1 - 65,535 characters 
        - TEXT
            - any length string (use if you need more than 255 characters)
        - We will use single quotes (') to indicate string values.
    - Date
        - DATE 
            - typically stored as YYYY-MM-DD
        - TIME 
            24-hour time HH:MM:SS
        - DATETIME
            - YYYY-MM-DD HH:MM:SS
        - Global severs are generally set to GMT
    - NULL
        - as the absence of value. **NOT ZERO**
