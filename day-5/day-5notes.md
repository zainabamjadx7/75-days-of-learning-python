# Day 5: Python Data Types 🐍

**Date**: Day 5 / 75 | **Difficulty**: ⭐ Beginner | **Time**: 30 mins

---

## 🎯 What You'll Learn Today

- Why every value in Python has a data type
- Using the `type()` function
- Understanding `str`, `int`, `float`, and `bool`
- Understanding `None` and `NoneType`
- Recognising type mismatches and why they cause errors
- Checking data types before using values
- Understanding common data type mistakes and fixes
- Using different data types inside f-strings
- Practising all five core data types

---

## 📚 Part 1: Why Every Value Has a Type

Day 4 introduced variables as labelled containers for values. Today's lesson answers a natural question: **what kind of value is actually inside the box?**

Every single value in Python belongs to a specific data type, and that type determines exactly what can be done with it.

### Why This Isn't Just Theory

Adding two numbers together works as expected. Adding two pieces of text behaves differently, and adding a number to a piece of text fails.

```python
print(2 + 2)       # 4
print('2' + '2')   # '22' (joins text, doesn't add)
print(2 + '2')     # TypeError!
```

---

## 💻 Part 2: The `type()` Function

`type()` is a built-in function, just like `print()`, that reveals exactly what data type a value or variable currently is.

```python
print(type('hello'))  # <class 'str'>
print(type(42))       # <class 'int'>
print(type(3.75))     # <class 'float'>
print(type(True))     # <class 'bool'>
```

### Reading `type()`'s Output

The output `<class 'str'>` simply means that the value belongs to the `str` (string) type.

The word `class` appears because, internally, every data type in Python is built using a class.

### Using `type()` as a Learning Tool

Whenever you are unsure what type a value is, wrapping it in `type()` is a quick way to confirm exactly what it is.

---

## 📝 Part 3: `str` — Text Data

`str` stands for **string** and represents any sequence of text characters. Strings are wrapped in either single or double quotes.

```python
name = 'A student'
print(type(name))  # <class 'str'>
```

### What Counts as a String?

- Words and sentences: `'Hello, World!'`
- Numbers written inside quotes: `'2026'` — this is text, NOT a number
- Even a single character: `'A'`
- An empty string with nothing inside: `''`

### ⚠️ The Most Common Day 5 Trap

`'20'` and `20` look almost identical but are entirely different types:

- `'20'` → `str`
- `20` → `int`

Confusing the two is one of the most common beginner errors.

---

## 🔢 Part 4: `int` — Whole Numbers

`int` stands for **integer** and represents whole numbers with no decimal point — positive, negative, or zero.

```python
age = 20
temperature = -5

print(type(age))  # <class 'int'>
```

### Integers Support Arithmetic

```python
print(10 + 5)  # 15
print(10 - 5)  # 5
print(10 * 5)  # 50
```

Full arithmetic operators, including division, powers, and remainders, are covered on Day 6. Today's focus is recognising and correctly typing integer values.

### No Commas Allowed

Unlike everyday writing, Python integers cannot contain commas as thousands separators.

```python
# Correct
1000000
```

---

## 🔢 Part 5: `float` — Decimal Numbers

`float` represents any number that includes a decimal point. It is commonly used for GPA, percentages, prices, and measurements.

```python
gpa = 3.75
price = 199.99

print(type(gpa))  # <class 'float'>
```

### A Whole Number Can Still Be a Float

```python
value = 5.0
print(type(value))  # <class 'float'>
```

The presence of a decimal point — even `.0` — is what makes Python classify a value as a `float` rather than an `int`.

### A Small Technical Quirk Worth Knowing

Because of how computers store decimals internally, calculations like `0.1 + 0.2` can sometimes display as:

```text
0.30000000000000004
```

This is a well-known floating-point behaviour, not a Python bug. The `:.2f` formatting from Day 3 can hide it in most everyday output.

---

## ✅ Part 6: `bool` — True and False

`bool` stands for **Boolean** and represents exactly one of two possible values:

- `True`
- `False`

Booleans are the foundation of every decision a program will make.

```python
is_enrolled = True
is_graduated = False

print(type(is_enrolled))  # <class 'bool'>
```

### Capitalisation Is Not Optional

```python
is_active = true
# NameError: name 'true' is not defined
```

`True` and `False` must always start with a capital letter. They are Python keywords, not ordinary words.

### Booleans Are Secretly Numbers Too

Internally, `True` behaves like `1` and `False` behaves like `0`.

```python
print(True + True)
# Output: 2
```

---

## ⚪ Part 7: `None` — The Absence of a Value

`None` is a special, unique value in Python representing the deliberate absence of any value.

It is not the same as zero, an empty string, or `False`.

```python
result = None

print(type(result))
# <class 'NoneType'>
```

### When `None` Is Actually Useful

- As a placeholder for a variable that will be given a real value later
- As the value a function returns when it has no meaningful result
- To represent genuinely missing data

### NOT THE SAME AS ZERO

These values may look similar at first, but Python treats them as distinct:

```python
0
''
False
None
```

Each has its own type and meaning.

---

## ⚠️ Part 8: Type Mismatches and Why They Crash Programs

A type mismatch happens when an operation is attempted between two values of incompatible types.

Python is strict about this by design — it will not guess what you meant, and it will raise an error instead.

```python
age = 20
message = 'I am ' + age + ' years old'
# TypeError: can only concatenate str (not "int") to str
```

### Why Python Refuses to Guess

Python stops immediately when incompatible types are combined instead of silently converting them. This helps prevent larger and harder-to-find bugs.

### The Fix: Explicit Conversion

```python
message = 'I am ' + str(age) + ' years old'
print(message)
# I am 20 years old
```

Wrapping `age` in `str()` explicitly converts it to text before joining it with the other text.

Full type conversion using `str()`, `int()`, and `float()` is covered in depth on Day 9.

---

## 🔍 Part 9: Checking Types Before Using Them

When you are unsure what type a value is, especially one coming from outside your own code, checking its type can prevent confusing errors.

```python
value = '20'

if type(value) == str:
    print('This is text, not a number')
```

If/else logic is formally introduced on Day 10. For now, simply recognise that `type()` combined with a comparison is a useful pattern for confirming assumptions about data.

### A Preview: `isinstance()`

A more advanced and flexible alternative to `type()` called `isinstance()` exists and is commonly used in professional code. It will be introduced properly later in the course.

---

## 🔍 Part 10: Common Data Type Mistakes & Fixes

### ❌ 1. Assuming Quoted Numbers Are Numbers

```python
age = '20'
print(age + 1)
# TypeError
```

**Fix:** Remove the quotes if a real number is intended.

```python
age = 20
print(age + 1)
```

---

### ❌ 2. Using Lowercase `true` or `false`

```python
is_ready = false
# NameError: name 'false' is not defined
```

**Fix:** Always capitalise `True` and `False`.

```python
is_ready = False
```

---

### ❌ 3. Confusing `None` With Empty or Zero

```python
value = None

if value == 0:
    print('Zero')
```

`None`, `0`, `''`, and `False` are different values and different types.

**Fix:** Use `is None` when specifically checking for `None`.

```python
if value is None:
    print('No value')
```

---

### ❌ 4. Forgetting `.0` Makes a Value a Float

```python
grade = 85.0

print(type(grade))
# <class 'float'>
```

Even though `85.0` looks like a whole number, Python treats it as a `float`.

**Fix:** Remember that the presence of a decimal point makes the value a `float`.

```python
grade = 85
print(type(grade))
# <class 'int'>
```

---

### ❌ 5. Mixing Different Data Types

```python
age = 20
message = 'I am ' + age + ' years old'
# TypeError
```

**Fix:** Convert the number to a string before joining it with text.

```python
age = 20
message = 'I am ' + str(age) + ' years old'

print(message)
# I am 20 years old
```

---

## 📋 Part 11: Quick Reference — All Five Types

| Type | Example | `type()` Output |
|---|---|---|
| **str** | `'hello'` | `<class 'str'>` |
| **int** | `42` | `<class 'int'>` |
| **float** | `3.75` | `<class 'float'>` |
| **bool** | `True` | `<class 'bool'>` |
| **NoneType** | `None` | `<class 'NoneType'>` |

These five types form the complete foundation for the data-related concepts introduced in this course.

---

## 🧩 Part 12: Data Types Inside f-Strings

Day 3 introduced f-strings without focusing deeply on data types. Now that all five types are understood, we can see how naturally f-strings handle them.

```python
name = 'A student'  # str
age = 20            # int
gpa = 3.75          # float
is_enrolled = True  # bool

print(f'{name} is {age} years old, GPA {gpa:.2f}, enrolled: {is_enrolled}')
```

### f-Strings Convert Automatically

No `str()` conversion is needed inside an f-string, even when the value is an `int` or `bool`.

f-strings automatically convert values to readable text for display.

---

## 🎯 Part 13: Today's Practice Task

Today's task is a hands-on tour of all five data types using the `type()` function.

### Instructions

1. Create one variable of each type:
   - A `str`
   - An `int`
   - A `float`
   - A `bool`
   - A value set to `None`
2. Print each variable's value.
3. Print each variable with `type()` to confirm the type.

### Expected Structure

```python
text_value = '...'
number_value = 0
decimal_value = 0.0
bool_value = True
empty_value = None

print(text_value, type(text_value))
print(number_value, type(number_value))
print(decimal_value, type(decimal_value))
print(bool_value, type(bool_value))
print(empty_value, type(empty_value))
```

> 💡 **Pro Tip:** `True` and `False` must have capital `T` and `F`. They are Python keywords, not regular words.

---

## 📖 Part 14: Key Terms Glossary

| Term | Meaning |
|---|---|
| **Data Type** | The category a value belongs to, determining what operations are valid on it |
| **`type()`** | A built-in function that reveals a value's data type |
| **str** | The text data type, usually wrapped in quotes |
| **int** | The whole-number data type, with no decimal point |
| **float** | The decimal-number data type |
| **bool** | The `True`/`False` data type |
| **NoneType** | The type of the special value `None`, representing no value at all |
| **Type Mismatch** | An error caused by combining incompatible data types |
| **Type Conversion** | Deliberately changing a value from one type to another |

---

## 🔄 Part 15: Day 4 vs Day 5 — What Changed?

| Aspect | Day 4 → Day 5 |
|---|---|
| **Core Skill** | Storing values in variables → Understanding what kind of value each one is |
| **New Tool** | `=` (assignment) → `type()` (inspection) |
| **Error Awareness** | `NameError` from missing variables → `TypeError` from mismatched types |
| **New Types** | Variables introduced → `str`, `int`, `float`, `bool`, and `NoneType` formally defined |
| **Groundwork** | Variables → Arithmetic, user input, and future data handling |

Day 4 answered:

> **"How do I store a value?"**

Day 5 answers:

> **"What exactly did I just store?"**

This distinction becomes important when real arithmetic, user input, and eventually datasets enter the picture.

---

## ❓ Part 16: Frequently Asked Questions

**Q: Do I need to memorise `type()` output exactly?**  
No. Recognising the type name — `str`, `int`, `float`, `bool`, or `NoneType` — is what matters.

**Q: Why does Python have both `int` and `float` instead of just one number type?**  
They represent whole numbers and decimal values differently. This distinction becomes important in statistics and machine learning.

**Q: Is there a type for dates or times?**  
Yes. Python provides a separate `datetime` module for dates and times.

**Q: What's the difference between `None` and an empty string `''`?**  
`None` represents no value at all, while `''` is a valid string containing zero characters.

**Q: What should I practise after today's task?**  
Try deliberately creating the `TypeError` from Part 8 by adding a string and a number directly, then fix it using `str()`. Seeing the error and resolving it builds stronger intuition.

---

## 🎓 Key Takeaways

1. ✅ Every Python value has a data type.
2. ✅ Use `type()` to check a value's data type.
3. ✅ `str` is used for text.
4. ✅ `int` is used for whole numbers.
5. ✅ `float` is used for decimal numbers.
6. ✅ `bool` contains `True` or `False`.
7. ✅ `None` represents the absence of a value.
8. ✅ Mixing incompatible types can cause a `TypeError`.
9. ✅ f-strings can display different data types naturally.
10. ✅ Understanding data types is essential for future Python and data analytics work.

---

**Ready for Day 6?**  
Next: Python Arithmetic & Operators! 🚀

