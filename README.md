# 🐍 Day 1 — Phase 1: Python Basics | AI/ML Journey

> Starting from scratch. Day 1 covers the absolute foundation every Python and ML developer needs before touching data or models.

---

## 📌 Topics Covered

### 1. 🔢 Variables & Assignment
A variable is a named container that stores a value in memory. Python figures out the type automatically — no need to declare it.

```python
# Creating variables
name = "Surya"
age = 22
height = 5.9
is_student = False

# Re-assign anytime
age = 23

# Multiple assignment at once
x, y, z = 10, 20, 30

# Same value to many variables
a = b = c = 0

# Swap two variables (Pythonic way!)
x, y = y, x
```

> 💡 **Rule:** Use `snake_case` for variable names — no spaces, no starting with a number.

---

### 2. 🗂️ Data Types

| Type | Example | Use Case |
|------|---------|----------|
| `int` | `42`, `-5`, `0` | Whole numbers, counts, ages |
| `float` | `3.14`, `-0.5` | Decimals, measurements, prices |
| `str` | `"hello"` | Text, names, messages |
| `bool` | `True`, `False` | Yes/no flags, conditions |
| `NoneType` | `None` | Empty / missing value |

```python
# Check any variable's type
print(type(name))     # <class 'str'>
print(type(age))      # <class 'int'>
print(type(height))   # <class 'float'>
```

#### Type Conversion (Casting)
```python
# int → float
float(10)        # 10.0

# float → int (truncates, doesn't round!)
int(9.8)         # 9

# str → int
int("100")       # 100

# int → str
str(25)          # "25"

# Boolean conversion
bool(0)          # False
bool(1)          # True
bool("")         # False
bool("hi")       # True
```

> 🛒 **Real-world example:**
> ```python
> price = "500"      # came from user input — it's a string!
> quantity = 2
> total = int(price) * quantity
> print(total)       # 1000
> ```

---

### 3. 🖨️ `print()` — Display Output

```python
# Basic print
print("Hello, World!")

# Print a variable
name = "Surya"
print("Name:", name)

# Print multiple values
print("Name:", name, "Age:", 23)

# f-string (most common & cleanest way)
print(f"My name is {name} and I am {22} years old")

# sep and end parameters
print("a", "b", "c", sep="-")   # a-b-c
print("Hello", end=" 👋")
```

#### f-strings — The Best Way to Format
```python
score = 95.678

print(f"Name: {name}")              # embed variable
print(f"Next year: {age + 1}")      # embed expression
print(f"Score: {score:.2f}")        # format decimal → 95.68
print(f"{name.upper()}")            # call methods inline → SURYA
```

---

### 4. ⌨️ `input()` — Get User Input

```python
# Basic input
name = input("Enter your name: ")
print(f"Hello, {name}!")

# input() always returns a STRING
age = input("Enter your age: ")
print(type(age))    # <class 'str'>

# Convert to int to use as a number
age = int(input("Enter your age: "))
print(f"In 5 years: {age + 5}")
```

> ⚠️ **Key point:** `input()` always returns `str`. Always convert when you need a number!

---

### 5. 💬 Comments

```python
# This is a single-line comment

"""
This is a
multi-line comment (also used as docstrings)
"""
```

---

## 🔑 Key Takeaways

- Variables store values — Python auto-detects the type
- 5 core data types: `int`, `float`, `str`, `bool`, `None`
- Use `type()` to inspect any variable
- Always cast `input()` output when you need a number
- f-strings are the cleanest way to format output

---

## 🚀 What's Next?

Day 2 → Operators, Conditions & Loops

---

*Part of my 100-day AI/ML learning journey. Follow along for daily notes, code, and concepts!*

`#Python` `#MachineLearning` `#AI` `#100DaysOfCode` `#DataScience` `#BeginnerPython`
