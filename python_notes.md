# Python

**Python** - very similar to english, it is not close to a machine langauge

## Interpretor vs Complier 

**Interpretor** - goes through line by ine and executes the code 

**Compiler** - reads all the code at once and then executes the entire script at once

When you download python, you are really downloading Cpython, which is an interpretor.  Cpython is coded using C, and ineterprets python code into Bite code line by line.  THis bite code is then run on the CPYTHON virtual machine, which ultimatley runs on our computers

```python

s = "And this is me typing my first python code"

print s

name = input("Your name?")
print("helllllooooooo " + name)

```


Python generally runs slower than other languages like C, Java - it should not be used for low level system appications - it should be used for developing, and is advantagious as its so widley used, and is easily readible 


# Data Types
**Fundemental Data types** - Values in python 

- int
- float
- bool
- str
- list
- tuple
- set
- dict
- Complex

**Classes** - custom data types 

**Specialized Data Types** - these come from modules, these are extentions to the language

**None** - null, this has no value

### int & Float

**int** - an integer
**float** - floating point number 

```python
print (2 + 4)
print (2 - 4)
print (2 / 4)
print (2 * 4)

print (type(6))
print (type(2 - 4))
print (type(2 / 4))
print (type(2 * 4))

```
Data type **float** takes up more space in memory than data type **int**

```python
print (type(9+9.9))
```
This will produce a data type of float, as an integer plus a float is a float

**Powers, division, modular**
```python
print (2 ** 4) 
print ( 5 // 4)
print (5 % 3)
```
// gets rounded down to remain as an integer

**modular** - is a remainder

**Math functions**
```python
print(round(3.1))
print(abs(-20))
```
round - rounds number

abs - gives the absolute value ( no negative values )


## Developer Fundementals 

**Dont learn the dictionary** - Learn by using the language, do not learn the edge case scinarios of the bat 

### Operator Precedance
20 + 3 * 4 

We complete this sum in order of operations, this follows **BIDMAS** 

### Storing data types in binary

```python 
print (bin(5))
```
the output of this is: 
```python
0b101
```
**b** - denotes binary number, and is how python stores numbers 

---
## Variables
**Variables** - are ways for us to stores data

**Nomenclatures**
- snake_case
- Start lowercase or underscore
- Letters, numbers, undersciores
- Case sensitive
- Cannot overwrite keywords - keywords in python already have meaning, therefore we cannot assign any value to the variable "print" as print already has a function

- varibles that are unique will be coloured white

Rapid variable application

```python
a,b,c = 1,2,3 
```

**Constants**
There are good conventions with variables, such as constants.  Though constants are variables, they should not be changed.  Constants are denoted by all Capital letters


```python
PI = 3.1459
```
The Variable "PI" has been declared as a constant due to capitalisations of the letters, therefore this value should not be changed

---
### Exprssions vs Statments

**Expressions** - x  = y + 10

**Statement** - y = 3

---

### Augmented assignment operator

```python 
some_value = 5 
some_value = some_value + 2
some_value += 2
some_value *=
```

To use augmented assigment operator, the variable must first have a value assisgned to it. 

---

### str

**str** - is just text, or a string of values

```python
first_name = 'double quotes'
last_name = "single quotes"
long_string = '''This has triple quotation marks.  
This allows me to continue typing over multiple lines

Tadaaa
'''

full_name = first_name + " " + last_name

```

**String concatenation** - this only works with string data types, you cannot mix data types


**type conversion** - converting data types 

```python
a = 1 
b = float(a)
c = type (b)
print (c)

```


---

### escape sequence 

```python
a = "\t\t This has been tabbed in. \n This is on a new line. \n \"This is in quotation marks\" "

print(a)
```

---

### Formatted strings

```python
name = 'John'
age =  33

print ('Hi ' + name + '. You are ' + str(age) + ' years old.')

print (f'hi {name}. You are {age} years old.')

print ('hi {0}. You are {1} years old.'.format(name, age))

print ('hi {1}. You are {0} years old.'.format(name, age))

print('Hi {new_name}. You are {age} years old.'.format(new_name='Sally', age=111))

```

---
### String Indexes

```python 
selfish = '01234567'

print(selfish[7]) # print index 7

print(selfish[1:4]) # print indexes 1 through 4

print(selfish[0:7:2]) # print indexes 0 - 7 and step over 2

print(selfish[3:]) # print all after index 3

print(selfish[:5]) # print all indexes before 5 

print(selfish[::2]) # print all indexes step over 2

print(selfish[-1]) # print all indexes starting from index 7

print(selfish[::-1]) # print all indexes step over -1 

```

---

### Immutability

**String Slicing** - selfish[start:stop:stepover]

**Strings in python are immutable** - they cannot be changed

```python
selfish = '01234567'

selfish = '8'
```
Because strings in python are immutable, once the string has a new value assigned to the old value is gone and replaced with the new value. 

Therefore: 

```python 
selfish = '01234567'
selfish[6] = 'tree'
```
Is not a feasible option, you cannot replace or change any value in the string, you can only replace the whole string. 


---

### Built in Functions and Methods




