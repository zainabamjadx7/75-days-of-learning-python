# Day 2: Your First Line & `print()` Basics 🐍

**Date**: Day 2 / 75 | **Difficulty**: ⭐ Beginner | **Time**: 30 mins

---

## 🎯 What You'll Learn Today

* What `print()` is and why it's essential
* Creating and running your first `.py` file in VS Code
* Understanding function syntax and string quotes
* Running code via VS Code Run Button & Terminal
* Common Day 2 beginner errors and fixes
* Writing comments and following Python file naming rules

---

## 📚 Part 1: What is `print()`?

`print()` is a built-in Python function that displays information on the screen. It is the most basic tool for a program to communicate output to the user.

```python
print('Hello, World!')
```

### How It Works Behind the Scenes

1. Python reads `print('Hello, World!')` from top to bottom.
2. It recognizes `print` as a built-in function.
3. It takes the text `'Hello, World!'` inside the brackets as the value to display.
4. It sends that text to standard output (the terminal).

---

## 💻 Part 2: Anatomy of the `print()` Statement

Every part of a `print()` statement has a specific purpose.

```python
print('I will be a Python developer')
```

* **`print`**: Built-in function name
* **`()`**: Parentheses — hold the arguments passed to the function
* **`''`**: Quotes — mark the start and end of a text string
* **`I will be a Python developer`**: The actual text content displayed

> 💡 **Note:** In Python 3, parentheses `()` are strictly required. Writing `print 'Hello'` will cause a syntax error.

---

## 📝 Part 3: Understanding String Quotes

Text wrapped inside quotes is called a **string**.

```python
# Single quotes
print('Hello there')

# Double quotes
print("Hello there")
```

### When to Use Which?

* **Single quotes (`'`)**: Default choice for plain text.
* **Double quotes (`"`)**: Preferred when text contains an apostrophe.
* **Rule**: Opening and closing quotes must always match!

Example:

```python
print("It's a great day")
```

---

## ⚙️ Part 4: Creating & Running Your First File

### Step 1: Create `hello.py`

1. Open VS Code and open your project folder.
2. Create a new file and name it `hello.py`.
3. Ensure the file extension is strictly `.py`.

### Step 2: Run the File

**Method 1 — VS Code Run Button**

Click the **Play / Run** button at the top-right corner.

**Method 2 — Terminal**

Open the integrated terminal (`Ctrl + ~`) and type:

```bash
python hello.py      # Windows
python3 hello.py     # macOS / Linux
```

> ⚠️ **Always Save First!** Press `Ctrl + S` (`Cmd + S` on Mac) before running.

---

## 🔢 Part 5: `print()` with Multiple Values

You can print multiple items in a single line by separating them with commas. Python automatically inserts spaces between them.

```python
print('My name is', 'Zainab', 'and I study Python')
```

**Output:**

```text
My name is Zainab and I study Python
```

Calling `print()` multiple times creates multi-line output:

```python
print('Line one')
print('Line two')
```

---

## 💬 Part 6: Comments in Python

Comments are notes ignored by Python when executing code. They start with the `#` symbol.

```python
# This is a comment - Python ignores this
print('Hello, World!')  # This line prints output
```

### Why Use Comments?

* Explain complex reasoning
* Temporarily disable lines of code while testing

---

## ⚠️ Part 7: Common Beginner Errors & Fixes

### ❌ Mistake 1: Missing Quotes (`NameError`)

**Wrong:**

```python
print(Hello)
```

Python thinks `Hello` is an undefined variable.

**Correct:**

```python
print('Hello')
```

---

### ❌ Mistake 2: Mismatched Quotes (`SyntaxError`)

**Wrong:**

```python
print('Hello")
```

Quotes must match.

**Correct:**

```python
print('Hello')
```

---

### ❌ Mistake 3: Missing Parentheses

**Wrong:**

```python
print 'Hello'
```

This causes a `SyntaxError` in Python 3.

**Correct:**

```python
print('Hello')
```

---

## 📁 Part 8: File Naming Rules

| Rule          | Description                | Example          |
| ------------- | -------------------------- | ---------------- |
| **Extension** | Must end with `.py`        | `hello.py`       |
| **Spaces**    | No spaces; use underscores | `my_code.py`     |
| **Casing**    | Lowercase preferred        | `app.py`         |
| **Keywords**  | Do not use reserved names  | Avoid `print.py` |

---

## 🎯 Part 9: Step-by-Step Practical Task

1. Open `hello.py` inside your project folder.
2. Write a `print()` statement with your name.
3. Write a second `print()` statement with your university/college.
4. Write a third `print()` statement with `"I will be a Python developer"`.
5. Save and run the program.

```python
# hello.py
print('Zainab Amjad')
print('UET Lahore')
print('I will be a Python developer')
```

---

## 📋 Part 10: Quick Reference

| Concept         | Code Example         | Notes                       |
| --------------- | -------------------- | --------------------------- |
| **`print()`**   | `print("Hello")`     | Displays text on screen     |
| **String**      | `'Text'` or `"Text"` | Text in quotes              |
| **Comma**       | `print('A', 'B')`    | Separates items with spaces |
| **Comment**     | `# Note`             | Ignored by Python           |
| **Run command** | `python filename.py` | Executes Python file        |

---

## 🎓 Key Takeaways

1. ✅ `print()` displays output on the standard console.
2. ✅ Strings require matching quotes (`'` or `"`)
3. ✅ Always save files (`Ctrl + S`) before running.
4. ✅ Python 3 requires parentheses `()` for function calls.
5. ✅ Use comments (`#`) to keep code documented.

---

**Ready for Day 3?**
Next: `print()` Mastery, `sep`, `end`, & f-strings! 🚀
