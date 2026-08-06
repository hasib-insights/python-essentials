###  Python Modules
A **module** is a **Python file** (`.py`) that contains code – like functions, classes, and variables –that you can **reuse** in other Python programs.
>  **Think of it like:** A module is a **toolbox**. Each toolbox has specific tools (functions) that you can take and use whenever you need them.
---
### Why Use Modules?

| Benefit | Explanation |
|---------|-------------|
| **Code Reuse** | Write once, use many times |
| **Organization** | Keep related code together |
| **Clean Code** | Avoid cluttering your main file |
| **Team Work** | Multiple people can work on different modules |
| **Easy Debugging** | Fix issues in one place |

---

### How to Create and Use a Module

### Step 1: Create a Python file (e.g., `mymodule.py`)

```python
# mymodule.py
def greet(name):
    return f"Hello, {name}! Welcome to Python!"

def add(a, b):
    return a + b

def multiply(a, b):
    return a * b

PI = 3.14159
```
### Step 2: Import and use it in another file (e.g., `main.py`)
```python
# main.py
import mymodule

print(mymodule.greet("Alice"))     # Hello, Alice! Welcome to Python!
print(mymodule.add(5, 3))          # 8
print(mymodule.multiply(4, 2))     # 8
print(mymodule.PI)                 # 3.14159
```
```python

                    HOW MODULES WORK                                 
──────────────────────────────────────────────────────────────────────

   📄 mymodule.py                     📄 main.py                     
   ┌──────────────────────┐          ┌─────────────────────────────┐ 
   │ def greet(name):     │          │ import mymodule             │ 
   │     return "Hello"   │          │                             │ 
   │                      │          │ print(mymodule.greet("Bob"))│ 
   │ def add(a, b):       │          │ print(mymodule.add(5, 3))   │ 
   │     return a + b     │          │                             │ 
   │                      │          │ Output:                     │ 
   │ def multiply(a, b):  │          │ Hello Bob!                  │ 
   │     return a * b     │          │ 8                           │ 
   └──────────────────────┘          └─────────────────────────────┘ 
   Module defines functions           Main file uses them         
                                                                      

```
### File Structure
```
my_project/
│
├── main.py           ← Your main program
├── mymodule.py       ← module
└── calculator.py     ← Another module
```

### Types of Modules
```
                 

                                                                      
   ┌─────────────────┐  ┌─────────────────┐  ┌─────────────────┐    
   │   Built-in      │  │   External      │  │   Custom        │    
   │   Modules       │  │   Modules       │  │   Modules       │    
   │                 │  │                 │  │                 │    
   │ • math          │  │ • numpy         │  │ mymodule.py     │    
   │ • random        │  │ • pandas        │  │ calculator.py   │    
   │ • datetime      │  │ • matplotlib    │  │ utils.py        │    
   │ • os            │  │ • scikit-learn  │  │ helpers.py      │    
   └─────────────────┘  └─────────────────┘  └─────────────────┘    
         │                      │                      │             
         └──────────────────────┼──────────────────────┘             
                                │                                     
                                ▼                                     
                    ┌─────────────────────────┐                      
                    │   import module_name    │                      
                    │   module_name.function()│                     
                    └─────────────────────────┘                      
                                                                      

```
---
### Different Ways to Import
```python
# 1. Import the Whole Module
import math

print(math.sqrt(25))   # 5.0
print(math.pi)         # 3.14159
```
```python
# 2. Import Specific Functions/Variables
from math import sqrt, pi

print(sqrt(25))   # 5.0
print(pi)         # 3.14159
```
```python
# 3. Import with an Alias (Nickname)
import math as m

print(m.sqrt(25))   # 5.0
print(m.pi)         # 3.14159
```
```python
# 4. Import Everything
from math import *

print(sqrt(25))   # 5.0
print(pi)         # 3.14159
```
