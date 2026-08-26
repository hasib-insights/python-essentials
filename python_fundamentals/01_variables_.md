## Variables
```python
variavle_name = value
```
## Basic variable declaration
```python
x = 5
y = "hasib"
print(x)
print(y)
```
out:
```text
5
Hasib
```
## print this variable
```python
x = 4       # x is of type int
x = "Hasib" # x is now of type str
print(x)
```
out: 
```
Hasib
```
## Casting
```python
x = str(3)    # string 
y = int(3)    # integer
z = float(3)  # floating

print(x)
print(y)
print(z)
```
out[]:
```
'3'
3
3.0
```
## Get the Type   
get the data type of a variable with the `type()` function.
```python
x = 5
y = "John"
print(type(x))
print(type(y))
```
out:
```
<class 'int'>
<class 'str'>
```
String variables can be declared either by using single or double quotes:
```python
x = "John"
# is the same as
x = 'John'
```
### Legal variable names

* A variable name must start with a letter or the underscore character  
* A variable name cannot start with a number  
* A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and _ )  
* Variable names are case-sensitive (age, Age and AGE are three different variables)  
* A variable name cannot be any of the Python keywords.

Example
```python
myvar = "Hasib"
my_var = "Hasib"
_my_var = "Hasib"
myVar = "Hasib"
MYVAR = "Hasib"
myvar2 = "Hasib"
my_variable_name = "Hasib"
```
## Illegal variable names
```python
2myvar = "Hasib"
my-var = "Hasib"
my var = "Hasib"
```
## Assign Multiple Values  
Many Values to Multiple Variables
```python
x, y, z = "Orange", "Banana", "Cherry"
print(x)
print(y)
print(z)
```
out:
```
Orange
Banana
Cherry
```
One Value to Multiple Variables
```python
x = y = z = "Orange"
print(x)
print(y)
print(z)
```
out:
```
Orange
Orange
Orange
```
## Unpack a list
```python
fruits = ["apple", "banana", "cherry"]
x, y, z = fruits
print(x)
print(y)
print(z)
```
out:
```
apple
banana
cherry
```
## Output Variables  
The `print()` function is often used to output variables.
```python
x = "Python is awesome"
print(x)
```
out:
```
Python is awesome
```
In the `print()` function, output multiple variables, separated by a comma(`,`):
```python
x = "Python"
y = "is"
z = "awesome"
print(x, y, z)
```
out:
```
Python is awesome
```
also use the `+` operator to output multiple variables:
```python
x = "Python "
y = "is "
z = "awesome"
print(x + y + z)
```
out:
```
Python is awesome
```
For numbers, the `+` character works as a mathematical operator:
```python
x = 5
y = 10
print(x + y)
```
out:
```
15
```
when try to combine a **string** and a **number** with the `+` operator, Python will give you an error:
 ```python
x = 5
y = "Hasib"
print(x + y)
```
out:
```
TypeError: unsupported operand type(s) for +: 'int' and 'str'
```
## Global Variables
Variables that are created outside of a function (as in all of the examples in the previous pages) are known as global variables.  
Global variables can be used by everyone, both inside of functions and outside.  
Example:
```python
x = "awesome"

def function_name():   #define a function 
  print("Python is " + x) #code block 

function_name() #call the function
```
### The global Keyword
Normally, when you create a variable inside a function, that variable is local, and can only be used inside that function.
To create a global variable inside a function, you can use the `global` keyword.
```python
def myfunc():
  global x
  x = "fantastic"

myfunc()

print("Python is " + x)
```
out:
```
Python is fantastic
```







