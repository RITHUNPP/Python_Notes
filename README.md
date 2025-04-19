
# 🐍 Python Notes for Notion

## 📌 Table of Contents
- [Basics](#basics)
- [Data Types](#data-types)
- [Control Flow](#control-flow)
- [Functions](#functions)
- [Object-Oriented Programming](#object-oriented-programming)
- [Modules & Packages](#modules--packages)
- [File Handling](#file-handling)
- [Error Handling](#error-handling)
- [Common Built-in Functions](#common-built-in-functions)
- [Libraries Overview](#libraries-overview)

---

## 🔰 Basics
```python
# Hello World
print("Hello, World!")

# Comments
# This is a single-line comment
"""
This is a 
multi-line comment
"""
```

---

## 🔢 Data Types
- **Numeric**: `int`, `float`, `complex`
- **Sequence**: `list`, `tuple`, `range`
- **Text**: `str`
- **Set**: `set`, `frozenset`
- **Mapping**: `dict`
- **Boolean**: `bool`
- **NoneType**: `None`

```python
x = 10           # int
y = 3.14         # float
text = "Python"  # str
lst = [1, 2, 3]  # list
tpl = (1, 2)     # tuple
s = {1, 2, 3}    # set
d = {"a": 1}     # dict
```

---

## 🔁 Control Flow

### if-elif-else
```python
x = 10
if x > 0:
    print("Positive")
elif x == 0:
    print("Zero")
else:
    print("Negative")
```

### Loops
```python
# For loop
for i in range(5):
    print(i)

# While loop
i = 0
while i < 5:
    print(i)
    i += 1
```

---

## 🧠 Functions
```python
def greet(name):
    return f"Hello, {name}"

print(greet("Rithun"))
```

- Default arguments
- *args and **kwargs

```python
def add(*args):
    return sum(args)

def show_info(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")
```

---

## 🧱 Object-Oriented Programming
```python
class Person:
    def __init__(self, name):
        self.name = name

    def greet(self):
        print(f"Hello, I am {self.name}")

p = Person("Rithun")
p.greet()
```

- Inheritance
- Encapsulation
- Polymorphism

---

## 📦 Modules & Packages
```python
# math module
import math
print(math.sqrt(16))

# Creating a module
# mymodule.py
def add(x, y):
    return x + y

# main.py
import mymodule
print(mymodule.add(3, 4))
```

---

## 📂 File Handling
```python
# Reading a file
with open("file.txt", "r") as f:
    print(f.read())

# Writing to a file
with open("file.txt", "w") as f:
    f.write("Hello, file!")
```

---

## ⚠️ Error Handling
```python
try:
    x = 1 / 0
except ZeroDivisionError:
    print("Cannot divide by zero!")
finally:
    print("Always executes")
```

---

## 🧰 Common Built-in Functions
- `len()`, `type()`, `range()`, `enumerate()`
- `map()`, `filter()`, `zip()`, `sorted()`

```python
numbers = [1, 2, 3]
squared = list(map(lambda x: x**2, numbers))
print(squared)
```

---

## 📚 Libraries Overview
- `NumPy` – Numerical computing
- `Pandas` – Data analysis
- `Matplotlib / Seaborn` – Visualization
- `Scikit-learn` – Machine learning
- `TensorFlow / PyTorch` – Deep learning
- `Flask / Django` – Web development

