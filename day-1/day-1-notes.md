# Day 1: Python Basics & Your First Program 🐍

**Date**: Day 1 / 75 | **Difficulty**: ⭐ Beginner | **Time**: 30 mins

---

## 🎯 What You'll Learn Today

- What Python is and why it's awesome
- Writing your first `print()` program
- Creating and using variables
- Understanding data types
- Getting user input

---

## 📚 Part 1: What is Python?

**Python** = A high-level programming language created in 1991

### Why Python?
✅ **Readable** - Code looks like English  
✅ **Versatile** - Used everywhere (data science, web, AI, automation)  
✅ **Beginner-friendly** - Simple syntax, less frustration  
✅ **Industry standard** - Google, Netflix, Amazon use it  

### Where Python Is Used
- Data Analytics (Pandas, NumPy)
- Machine Learning (TensorFlow, PyTorch)
- Web Development (Django, Flask)
- Automation & Scripting
- Finance & Scientific Computing

---

## 💻 Part 2: Your First Program

### The `print()` Function

**Display text to the screen:**

```python
print("Hello, World!")
print("I am learning Python!")
```

**Output:**
```
Hello, World!
I am learning Python!
```

### Multiple Lines

```python
print("ZAINAB AMJAD")
print("UET Lahore")
print("I will be a Python developer")
```

**Each `print()` creates a new line!**

---

## 📝 Part 3: Variables - Store Values

A **variable** = a named container for storing data

```python
name = "Zainab"
age = 20
height = 5.6
is_student = True
```

### Variable Naming Rules

✅ **Valid:**
- `name`, `user_name`, `age`, `_private`

❌ **Invalid:**
- `1name` (can't start with number)
- `user-name` (no hyphens)
- `user name` (no spaces)
- `class` (reserved keyword)

**Convention:** Use `snake_case` (lowercase_with_underscores)

---

## 🔢 Part 4: Data Types

Python has different types of values:

### 1. **String (str)** - Text
```python
name = "Zainab"
message = 'Hello Python'
```

### 2. **Integer (int)** - Whole Numbers
```python
age = 20
year = 2024
```

### 3. **Float (float)** - Decimals
```python
height = 5.6
price = 99.99
```

### 4. **Boolean (bool)** - True/False
```python
is_student = True
is_working = False
```

### Check Data Type
```python
print(type("Zainab"))   # <class 'str'>
print(type(20))         # <class 'int'>
print(type(5.6))        # <class 'float'>
print(type(True))       # <class 'bool'>
```

---

## 🖨️ Part 5: Printing with Variables

### Method 1: Concatenation (Joining Strings)

```python
name = "Zainab"
print("Hello, " + name)  # Output: Hello, Zainab
```

⚠️ **Problem:** Can't add string + number directly!
```python
age = 20
print("Age: " + age)  # ❌ ERROR!
print("Age: " + str(age))  # ✅ Convert with str()
```

### Method 2: f-strings (Better!) ⭐

```python
name = "Zainab"
age = 20
print(f"I am {name}, {age} years old")
# Output: I am Zainab, 20 years old
```

**f-strings work with any data type - no conversion needed!**

```python
height = 5.6
print(f"Height: {height}m")  # Works perfectly!
```

---

## ⌨️ Part 6: User Input

The `input()` function gets text from the user:

```python
name = input("What is your name? ")
print(f"Hello, {name}!")
```

**Run this:**
```
Input: What is your name? Zainab
Output: Hello, Zainab!
```

### Important: `input()` Returns String

```python
age = input("Your age: ")  # User types: 20
print(type(age))          # Output: <class 'str'> (text, not number!)

# To do math, convert to int:
age = int(input("Your age: "))
print(age + 5)  # Now it works!
```

### Converting Data Types

```python
# String to Integer
num_str = "25"
num_int = int(num_str)
print(num_int + 5)  # Output: 30

# String to Float
price_str = "99.99"
price_float = float(price_str)
print(price_float * 2)  # Output: 199.98

# Number to String
age = 20
age_str = str(age)
print("Age: " + age_str)  # Works now!
```

---

## ⚡ Part 7: Simple Math with Variables

```python
num1 = 10
num2 = 5

sum_result = num1 + num2        # 15
difference = num1 - num2        # 5
product = num1 * num2           # 50
division = num1 / num2          # 2.0
power = num1 ** 2               # 100

print(f"10 + 5 = {sum_result}")
print(f"10 - 5 = {difference}")
print(f"10 * 5 = {product}")
print(f"10 / 5 = {division}")
print(f"10 ** 2 = {power}")
```

---

## ⚠️ Part 8: Common Beginner Mistakes

### ❌ Mistake 1: Forgetting Quotes
```python
# Wrong
name = Zainab  # Python thinks Zainab is a variable!
# Correct
name = "Zainab"
```

### ❌ Mistake 2: Confusing = with ==
```python
# Assignment
x = 5  # Set x to 5

# Comparison (we'll use this later)
x == 5  # Is x equal to 5? (Yes/No question)
```

### ❌ Mistake 3: Case Sensitivity
```python
name = "Zainab"
print(name)   # ✅ Works
print(Name)   # ❌ ERROR - Python is case-sensitive!
```

### ❌ Mistake 4: Can't Add String + Number
```python
# Wrong
age = 20
print("My age is " + age)  # ❌ ERROR

# Correct
print("My age is " + str(age))  # ✅ Convert first
# Or better:
print(f"My age is {age}")  # ✅ Use f-string
```

---

## 🎯 Part 9: Step-by-Step Tutorial

### Step 1: Open VS Code and Create `hello.py`

```python
# hello.py
print("Hello, Python!")
```

### Step 2: Run It
```bash
python hello.py
```

**Output:**
```
Hello, Python!
```

### Step 3: Create a Larger Program

```python
# my_profile.py
name = "Zainab"
university = "UET Lahore"
goal = "Become a Python developer"

print(f"My name is {name}")
print(f"I study at {university}")
print(f"My goal: {goal}")
```

### Step 4: Add User Input

```python
# interactive.py
name = input("What's your name? ")
age = int(input("What's your age? "))
city = input("Which city? ")

print(f"\n{name} is {age} years old from {city}")
```

---

## 📋 Part 10: Quick Reference

| Concept | Example | Notes |
|---------|---------|-------|
| print() | `print("Hi")` | Display output |
| Variable | `name = "Ali"` | Store data |
| String | `"Hello"` or `'Hello'` | Text (in quotes) |
| Integer | `20`, `-5`, `0` | Whole numbers |
| Float | `3.14`, `5.6` | Decimal numbers |
| Boolean | `True`, `False` | Yes/No values |
| input() | `age = input("Age? ")` | Get user input |
| f-string | `f"{name} is {age}"` | Format text |
| type() | `type(5)` | Check data type |
| int() | `int("20")` | Convert to integer |
| str() | `str(20)` | Convert to string |

---

## 🎓 Key Takeaways

1. ✅ `print()` displays output
2. ✅ Variables store values
3. ✅ 4 main data types: str, int, float, bool
4. ✅ f-strings format text elegantly
5. ✅ `input()` gets user data (returns string)
6. ✅ Convert types: `int()`, `str()`, `float()`
7. ✅ Use meaningful variable names
8. ✅ Test code frequently

---

**Ready for Day 2?** Next: Operators & Expressions! 🚀

---

