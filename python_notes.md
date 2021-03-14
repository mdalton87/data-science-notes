# 1/12/2021
## **Data Types**
- **bool**: boolean values, either True or False; an answer to a yes/no question
- **str** (**string**) a sequence of characters "strung" together
- **int**: whole, or counting numbers
- **float**: decimal numbers
- **list**: an ordered sequence of objects
- **dict**: a collection of values that have names
- **NoneType**: a special value that indicates absence of a value

## **Variables**
- A variable is a way to assign a name to a value. Variables are created by choosing a valid identifier and using the assignment operator, =

### **Naming convention**
- UpperCamelCase for class names
- CAPITALIZED_WITH_UNDERSCORES for constants
- lowercase_separated_by_underscores for other names

## **Booleans**
- There are 2 possible boolean values, **True** or **False** 
- Booleans can be thought of as the answer to a yes or no question
- Can be compared with the **==** and **!=** operators
- Can be combined with the **AND** and **OR** operators
## **Numbers**
- Can be **int** (integer) or **float**
    - **int** cannot have decimal places in them, while **floats** can

### **Mathmatical Operators**

- Addition, 	+
- Subtraction, 	-
- Multiplication, 	*	
- Division, 	/
- Exponentiation,	**

### **Comparison Operators**

- '==' - Equal to	
- '!=' - Not equal t
- '>' -	Greater than
- '<' -	Less than	
- '>=' - Greater than or equal to	
- '<=' - Less than or equal to

## **Strings** 
- Delimeted with either single (' ') or double quotes (" ")
    - *It is a good practice to pick one type of quotes for your code base and stick to it, either single or double*
- print('Here is a single quote --> \' <-- ')
- print("Here is a single quote --> ' <-- ")
- print()
- print("Here is a double quote --> \" <--")
- print('Here is a double quote --> " <--')
- print()
- print('Newlines are indicated by the character "n" preceded by a backslash, like so')
- print()
- print('This string\ncontains a newline')
    - Here is a single quote --> ' <--
    - Here is a single quote --> ' <--
    - 
    - Here is a double quote --> " <--
    - Here is a double quote --> " <--
    - 
    - Newlines are indicated by the character "n" preceded by a backslash, like so
    - 
    - This string
    - contains a newline

### **String Formatting**
- **%** formatting: a little older, but still fairly common
- **.format**: a newer way to format strings
- **f-strings**: introduced in python 3.6; comparable to string interpolation in other languages
```
name = 'World'
'Hello, %s!' % name

'Hello, World!'
'Hello, {}!'.format(name)

'Hello, World!'
f'Hello {name}!'

'Hello World!'
```
### **String Methods**
- **.lower** and **.upper:** convert the string to all lower or upper case
- **.strip:** remove any leading and trailing whitespace from the string
- **.isdigit**: test whether or not the string is a number
- **.split:** convert a string to a list
- **.join**: convert a list to a string
```
s = '   Hello, Codeup!   '
s.lower()

'   hello, codeup!   '
s.strip()

'Hello, Codeup!'
s.isdigit()

False
'123'.isdigit()

True
s.strip().split(', ')

['Hello', 'Codeup!']
', '.join(['one', 'two', 'three'])

'one, two, three'
```
## **Lists**

- Hold values in numeric order
- Can hold ANY data type (including other lists)
- Spreadsheets or db tables are lists of lists
```
beatles = ["John", "George"', "Paul"]
beatles.append("Ringo")

beatles.remove("Paul")