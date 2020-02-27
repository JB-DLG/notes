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

<br>

---
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

<br>

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

<br>

---
## Exprssions vs Statments

**Expressions** - x  = y + 10

**Statement** - y = 3

<br>

---

## Augmented assignment operator

```python 
some_value = 5 
some_value = some_value + 2
some_value += 2
some_value *=
```

To use augmented assigment operator, the variable must first have a value assisgned to it. 

---

<br>

## str (strings)

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

<br>

---

## Escape Sequence 

```python
a = "\t\t This has been tabbed in. \n This is on a new line. \n \"This is in quotation marks\" "

print(a)
```
<br>

---

## Formatted strings

```python
name = 'John'
age =  33

print ('Hi ' + name + '. You are ' + str(age) + ' years old.')

print (f'hi {name}. You are {age} years old.')

print ('hi {0}. You are {1} years old.'.format(name, age))

print ('hi {1}. You are {0} years old.'.format(name, age))

print('Hi {new_name}. You are {age} years old.'.format(new_name='Sally', age=111))

```
<br>

---
## String Indexes

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

<br>

---

## Immutability

**String Slicing** - selfish[start:stop:stepover]

**Strings in python are immutable** - they cannot be changed

```python
selfish = '01234567'

selfish = '8'
```
Because strings in python are immutable, once the string has a new value assigned to the old value is gone and replaced with the new value. 

Therefore below **Is not a feasible option**: 

```python 
selfish = '01234567'
selfish[6] = 'tree'
```
You cannot replace or change any value in the string, you can only replace the whole string. 

<br>

---

## Built in Functions and Methods

There a built in methods in python. 

You call these methods by prefixing an existing method name with a dot.

```python 
variable = "this is myvariable"

print(variable.upper())

print(variable.capitalize())

print(variable.replace("s", "poo")

remember = variable.replace("this", "Magic").upper()

print(remember)

```
Methods:

**upper** - will capitalise entier string. 

**capitalize** - will capitalise only the first letter in the string. 

**replace** - will repace the all of matching  segment of the sting with another selected word. 

**Remeber** - Strings are immutable, they cannot be changed, therefore any changes made to the string using methods are transient.  

<br>

---

## Booleans

Boolean values are simply **TRUE** or **FALSE**

```python 
print(bool(1))
print(bool(0))

```
These can be used for functional programming

<br>
---
### Type Conversion

```
import datetime

a = input("year")
b = input ("Month")
c = input ( "day")

birth_date = datetime.datetime(int(a), int(b), int(c))

print(birth_date)

from datetime import date

today = date.today()

```


## Comments in python

```python

# this is a comment

var = "this is my variiable" # and this is my comment

```

<br>

---

## Passwords 

```python
name = input ("name: ")
password = input ("enter password: ")
password_length  = int(len(password))
hidden_password = "*" * password_length

print(f'{name}, your password {hidden_password} is {password_length} characters long')

```

<br>

---
## List

**list** - an ordered seqeucen of object that can be of any type - lists are like arrays **but not exactly**

you can hold different datatypaes in lists

```python 
li1 = [1,2,3,4,5,6]
li2 = ['a',1.2,3,True]

print(li2[3])
print(li2[2:4])
print(li2[0::2])


```

Lists are mutable in the sence that the objects in a specific location in the list can be replaced

```python
li2 = ['a',1.2,3,True]

li2[0]="tree"
print(li2)
```
**list slicing** - this essentially creates a copy of the list, meaning the original list has not been changed, only the copy had been modified

```python
li2 = ['a',1.2,3,True]

print(li2[0:3]) # this is a copy of the list
print(li2) # this list is the original

```

**Important** - If you do not slice a list, then you are modifying it

```python
li2 = ['a',1.2,3,True]

new_list = li2
new_list[0] = "CHANGE"
print(new_list)
print(li2)

### What this does is make the variable new_list equal to the list li2.  So if we modify the variable new_list we are also modifying the li2.  The equal sign is a two way street. 

### See below: 

new_list = li2
new_list[0] = "CHANGE"
print(new_list)
print(li2)

li2[2] = "LOOK AT ME"
print(new_list)

### any modifications made to either li2 or new_list will appear when either are printed to the console

```

**Copying Lists** - To avoid the issue above create a copy of a list, therefore preserving the original and allowing the copy to be modified.
<br>

We use list slicing, which allows us to copy the entire list to a new variable

```python
new_list2 = li2[:]

print(new_list2)
```

## Matrix 

**multi-dimensional arrays** - an array inside an array

```python
matrix = [
    [1,2,3], 
    [4,5,6], 
    [7,8,9]
]

for num in matrix:
  print(num)
```

## List Methods

```python

basket = [1,2,3,4,5,6]
print(len(basket))

## Adding - append

new_list = basket.append(100) ## this does not have any value, it is simply a method appening a value to a list, therefore if we print it...

print(new_list) ## if we print it has a value of nonee
print(basket) ## Whereas, when we print the orignial list, we can see the appended value has been added.

## Instead of applying the method to a variable, we can execute the variable on its own. 

basket.append(200)

new_list = basket 
print(new_list)
print(basket)  ## however, now we incure the same problem as the copying of lists detailed above

## Insert 

basket.insert(3, 300)
print(basket)

## Extend

basket.extend([100,101])
print(basket)

## Removing

basket.pop()
print(basket) ##  pop will remove the last value in the list from the list 

basket(0)
print(basket) ## This will remove the first value

## remove

basket.remove(4)
print(basket) ## this removes this value from the list

## returning Poped value
poped_value = basket.pop(3) ## this variable is made = to the value that was poped from the list
print(poped_value)  ## this returns the value that was poped


## Clear
basket.clear()
print(basket)  ## this clears the list of all values


```





