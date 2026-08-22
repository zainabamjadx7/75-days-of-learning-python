**Date**: Day 3 / 75 | **Difficulty**: ⭐ Beginner | **Time**: 30 mins

# Python `print()` Function & f-Strings Guide

## 1. Overview & Basics

The `print()` function in Python is used to display output on the terminal/screen. Besides simple output, its advanced parameters and formatting options allow you to control how the output appears.

```python
print('Hello, World!')
```

---

## 2. The `sep` Parameter

When we pass multiple values to `print()` using commas (`,`), Python automatically adds a space between them. The `sep` parameter allows us to change the default separator.

```python
# Default space separator
print('a', 'b', 'c')
# Output: a b c

# Custom separator '-'
print('a', 'b', 'c', sep='-')
# Output: a-b-c

# Empty separator (no space)
print('a', 'b', 'c', sep='')
# Output: abc

# Date formatting example
print(2026, 7, 1, sep='/')
# Output: 2026/7/1
```

---

## 3. The `end` Parameter

By default, every `print()` statement adds a new line (`\n`) after the output. The `end` parameter allows us to change this behavior.

```python
# Joining output on the same line
print('Hello', end=' ')
print('World')
# Output: Hello World

# Custom ending
print('Loading', end='...')
# Output: Loading...
```

> **Key Difference:**
>
> * `sep` → Controls the separator **between values**.
> * `end` → Controls what appears at the **end of the print statement**.

---

## 4. Combining `sep` and `end`

You can use both `sep` and `end` in the same `print()` call:

```python
print('Python', 'is', 'fun', sep='-', end='!\n')
# Output: Python-is-fun!
```

---

## 5. Escape Characters

Escape characters (`\`) are used to include special characters inside strings:

| Character | Description                      |
| --------- | -------------------------------- |
| `\n`      | Newline (moves to the next line) |
| `\t`      | Tab (horizontal space)           |
| `\'`      | Single quote                     |
| `\"`      | Double quote                     |
| `\\`      | Backslash                        |

```python
print('Line one\nLine two')
```

---

## 6. Introduction to f-Strings

f-strings are a simple and efficient way in modern Python to embed variables and values directly inside text.

```python
city = 'Lahore'
print(f'I live in {city}')
# Output: I live in Lahore
```

---

## 7. Formatting Numbers in f-Strings

To print numbers in a specific format, such as decimal places or percentages, use a colon `:` followed by a format specifier.

| Specifier | Description                     | Example Output |
| --------- | ------------------------------- | -------------- |
| `:.2f`    | Round to 2 decimal places       | `3.86`         |
| `:.0f`    | Round to a whole number         | `4`            |
| `:,`      | Thousands separator             | `1,500,000`    |
| `:.1%`    | Percentage with 1 decimal place | `85.5%`        |

```python
gpa = 3.85921
print(f'GPA: {gpa:.2f}')
# Output: GPA: 3.86
```

---

## 8. Formatted Profile Card Example

```python
name = "Ali"
roll_no = "2026-CS-001"
gpa = 3.859
city = "Lahore"

print("-" * 25)
print(f"Name:    {name}")
print(f"Roll No: {roll_no}")
print(f"GPA:     {gpa:.2f}")
print(f"City:    {city}")
print("-" * 25)
```

**Output:**

```text
-------------------------
Name:    Ali
Roll No: 2026-CS-001
GPA:     3.86
City:    Lahore
-------------------------
```

---

## 9. Common Mistakes to Avoid

1. **Forgetting the `f`:** `print('GPA: {gpa}')` will print the text itself instead of the variable's value. Correct: `print(f'GPA: {gpa}')`.
2. **Missing braces:** Not closing `{` with `}` results in a `SyntaxError`.
3. **Undefined Variable:** Using a variable in an f-string before defining it results in a `NameError`.

---

## 10. Summary / Quick Glossary

* **`sep`**: Separator parameter between arguments.
* **`end`**: Ending character parameter after `print()` completes.
* **f-string**: A string prefixed with `f''` that allows expressions to be embedded inside `{}`.
* **`:.2f`**: Formats a floating-point number to 2 decimal places.

## This is it!

## See you Tomorrow
