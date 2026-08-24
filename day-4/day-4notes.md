# Day 4: Python Variables 🐍

**Date**: Day 4 / 75 | **Difficulty**: ⭐ Beginner | **Time**: 30 mins

---

## 🎯 What You'll Learn Today

* What a variable is and why it's essential
* The assignment operator (`=`) and reading it correctly
* Creating and printing your first variables
* Strict Python variable naming rules and `snake_case` style
* Variable reassignment and multiple assignment in one line
* Variables vs. Literals and how Python stores data in memory
* Building a personal info program using f-strings

---

## 📚 Part 1: What Is a Variable?

A variable is a named container that stores a value in your computer's memory so it can be used, changed, or displayed later. Without variables, every value would need to be typed out literally every time.

### A Real-World Analogy

Think of a variable as a labeled box on a shelf. The label (variable name) stays the same, but the content inside (value) can be swapped out whenever needed.

```python
city = 'Lahore'
print(f'I live in {city}')
```

---

## 💻 Part 2: The Assignment Operator (`=`)

In Python, `=` does NOT mean mathematical equality. It is the **Assignment Operator** — it takes the value on the right and stores it in the variable on the left.

```python
age = 20
```

> 💡 **Pro Tip:** Read `=` as **"gets set to"** (e.g., *age gets set to 20*) to avoid confusion with mathematical equality (`==`).

---

## 📝 Part 3: Creating Your First Variables

No keywords or declarations are needed to create a variable in Python — simply name it and assign a value.

```python
name = 'A student'
age = 20
city = 'Lahore'
gpa = 3.75

print(name)
print(age)
print(f"{name} is {age} years old and lives in {city}.")
```

---

## ⚠️ Part 4: Variable Naming Rules & Conventions

### Strict Python Naming Rules

Breaking these rules causes an immediate `SyntaxError`:

| Rule                               | Valid Example              | Invalid Example        |
| :--------------------------------- | :------------------------- | :--------------------- |
| Start with letter or underscore    | `name` ✅                   | `2name` ❌              |
| No starting with digits            | `age2` ✅                   | `22age` ❌              |
| Only letters, numbers, underscores | `roll_no` ✅                | `roll-no` ❌            |
| No spaces allowed                  | `first_name` ✅             | `first name` ❌         |
| Case-sensitive                     | `Age` & `age` are distinct | —                      |
| No Python keywords                 | `user_class` ✅             | `class`, `for`, `if` ❌ |

### `snake_case` Style Convention

Python developers use `snake_case` (all lowercase separated by underscores) for variables:

* `my_name = 'Zainab'` ✅ *(Pythonic)*
* `myName = 'Zainab'` ❌ *(Works, but not standard)*
* `MyName = 'Zainab'` ❌ *(Reserved for classes)*

---

## 🔄 Part 5: Reassigning Variables & Multiple Assignment

### Variable Reassignment

A variable's value can be overwritten at any time. Python forgets the old value unless saved elsewhere.

```python
score = 70
print(score) # Output: 70

score = 85
print(score) # Output: 85
```

### Multiple Assignment in One Line

Assign values to multiple variables compactly:

```python
# Same value to multiple variables
x = y = z = 0

# Different values in one line
name, age, city = 'A student', 20, 'Lahore'
```

---

## 🧩 Part 6: Variables vs. Literals

* **Literal**: A fixed value written directly in code (e.g., `'Hello'`, `20`).
* **Variable**: A named reference pointing to a memory location holding a value.

```python
# Using literal directly
print('Hello')

# Using variable
greeting = 'Hello'
print(greeting)
```

---

## 🔍 Part 7: Common Beginner Mistakes & Fixes

### ❌ 1. Using a Variable Before Defining It

```python
print(score) # NameError: name 'score' is not defined
score = 85
```

*Fix*: Always assign the variable before using it.

### ❌ 2. Forgetting Quotes Around Strings

```python
city = Lahore # NameError: name 'Lahore' is not defined
```

*Fix*: Text values must be wrapped in quotes (`city = 'Lahore'`).

### ❌ 3. Spelling & Case Typos

```python
citty = 'Lahore'
print(city) # NameError: name 'city' is not defined
```

*Fix*: Variable names must match exact casing and spelling.

---

## 🎯 Part 8: Practical Program Example

```python
# Personal Info Program
name = 'Zainab'
age = 20
city = 'Jhelum'
university = 'UET Lahore'
gpa = 3.75
roll_no = '2025-CE-01'
semester = 2
subject = 'Computer Engineering'

# Output displaying formatted info
print(f"Name: {name}")
print(f"Age: {age}")
print(f"City: {city}")
print(f"University: {university}")
print(f"GPA: {gpa:.2f}")
print(f"Roll No: {roll_no}")
print(f"Semester: {semester}")
print(f"Subject: {subject}")
```

---

## ❓ Frequently Asked Questions (FAQ)

**Q: Do variable names need to describe their content exactly?**
Yes! Clear names like `gpa` make code self-explanatory compared to vague names like `x`.

**Q: Can a variable name be a single letter?**
Technically yes, but only for short counters (like `i` in loops). Descriptive names are preferred for actual data.

**Q: What happens if I accidentally use a keyword as a variable name?**
Python immediately raises a `SyntaxError` before running.

**Q: Is it bad practice to reassign a variable to a different data type?**
Python allows it, but it's discouraged in real projects to prevent confusing bugs.

---

## 📋 Quick Reference Glossary

| Term             | Meaning                                               |
| :--------------- | :---------------------------------------------------- |
| **Variable**     | A named container that stores a value in memory.      |
| **Assignment**   | Storing a value in a variable using `=`.              |
| **Reassignment** | Overwriting an existing variable's stored value.      |
| **`snake_case`** | Lowercase words joined by underscores.                |
| **Keyword**      | Reserved words in Python grammar (e.g., `if`, `for`). |
| **Literal**      | A fixed value written directly in code.               |

---

## ✅ Checklist - Day 4 Complete When:

* [ ] Understood what variables are and how memory storage works.
* [ ] Practiced `snake_case` variable creation.
* [ ] Avoided using reserved Python keywords as names.
* [ ] Built a complete personal info program using 8 variables and f-strings.

---

**Ready for Day 5?** Next: Deep Dive into Data Types (`str`, `int`, `float`, `bool`)! 🚀
## See you Tomorrow!
