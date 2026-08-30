# Day 6: Python Numbers & Math 🐍

**Date**: Day 6 / 75 | **Difficulty**: ⭐ Beginner | **Time**: 30 mins
---
## 🎯 What You'll Learn Today
* `int` and `float`
* Python arithmetic operators
* `/` vs `//`
* Modulus `%` and exponent `**`
* Order of operations
* Shorthand operators
* Mixing `int` and `float`
* Common math mistakes
* Real-world formulas
* Percentage calculations
---
## 📚 Part 1: Numbers in Python
Python mainly uses two number types:
* **`int`** → Whole numbers
* **`float`** → Decimal numbers
```python
age = 20
gpa = 3.75
print(type(age))  # int
print(type(gpa))  # float
```
Python can use these values for calculations.
---
## ➕ Part 2: Arithmetic Operators
Python has seven main arithmetic operators:

| Operator | Meaning        | Example         |
| -------- | -------------- | --------------- |
| `+`      | Addition       | `7 + 3 → 10`    |
| `-`      | Subtraction    | `7 - 3 → 4`     |
| `*`      | Multiplication | `7 * 3 → 21`    |
| `/`      | True Division  | `10 / 3 → 3.33` |
| `//`     | Floor Division | `10 // 3 → 3`   |
| `%`      | Remainder      | `10 % 3 → 1`    |
| `**`     | Exponent       | `2 ** 3 → 8`    |

---
## ➗ Part 3: `/` vs `//`
### `/` — True Division
Returns a `float`.
```python
print(10 / 2)
# 5.0
```
### `//` — Floor Division
Rounds down to the nearest whole number.
```python
print(10 // 3)
# 3

print(-7 // 2)
# -4
```

> 💡 `//` means floor division, not normal rounding.
---
## 🔢 Part 4: Modulus `%`

`%` returns the **remainder** after division.
```python
print(10 % 3)
# 1
```
It is useful for checking even and odd numbers:

```python
number = 8
print(number % 2)
# 0 → Even
```

```python
number = 7
print(number % 2)
# 1 → Odd
```
---
## ⚡ Part 5: Exponents `**`
`**` is used to calculate powers.
```python
print(2 ** 3)
# 8

print(5 ** 2)
# 25
```
Square root:
```python
print(16 ** 0.5)
# 4.0
```
---
## 🧮 Part 6: Order of Operations
Python follows **PEMDAS**:
* **P** → Parentheses
* **E** → Exponents
* **M/D** → Multiplication / Division
* **A/S** → Addition / Subtraction

```python
print(2 + 3 * 4)
# 14
```
Use parentheses when needed:
```python
print((2 + 3) * 4)
# 20
```
> 💡 When in doubt, use parentheses to make your calculation clear.
---
## 🔄 Part 7: Shorthand Operators
Shorthand operators update a variable easily.
```python
score = 10

score += 5
print(score)
# 15
```

| Shorthand | Equivalent  |
| --------- | ----------- |
| `x += 5`  | `x = x + 5` |
| `x -= 5`  | `x = x - 5` |
| `x *= 5`  | `x = x * 5` |
| `x /= 5`  | `x = x / 5` |

---

## 🔢 Part 8: Mixing `int` and `float`

Python allows `int` and `float` to work together.

```python
result = 5 + 2.5

print(result)
# 7.5

print(type(result))
# float
```

When a `float` is involved, the result is generally a `float`.

---

## 🔍 Part 9: Common Math Mistakes & Fixes

### ❌ 1. Confusing `/` and `//`

```python
average = 17 // 2
print(average)
# 8
```
**Fix:** Use `/` for a precise decimal result.
```python
average = 17 / 2
print(average)
# 8.5
```

---
### ❌ 2. Forgetting Operator Precedence

```python
result = 2 + 3 * 4
# 14
```

**Fix:** Use parentheses when addition should happen first.

```python
result = (2 + 3) * 4
# 20
```

---

### ❌ 3. Dividing by Zero

```python
print(10 / 0)
# ZeroDivisionError
```

**Fix:** Make sure the divisor is not zero.

```python
print(10 / 2)
# 5.0
```

---

### ❌ 4. Using `^` for Exponents

```python
print(2 ^ 3)
```

`^` is **not** the exponent operator in Python.

**Fix:** Use `**`.

```python
print(2 ** 3)
# 8
```

---

### ❌ 5. Using `=` for Comparison

```python
score = 10
```

`=` means **assignment**.

**Fix:** Remember:

```text
=   → Assignment
==  → Comparison
```

---

## 🧩 Part 10: Real-World Formula — Circle Area

Formula:

```text
Area = π × radius²
```

Python:

```python
pi = 3.14159
radius = 5

area = pi * (radius ** 2)

print(f'Area: {area:.2f}')
# Area: 78.54
```

---

## 💰 Part 11: Compound Interest

Formula:

```text
Final Amount = Principal × (1 + Rate) ^ Time
```

Python:

```python
principal = 100000
rate = 0.05
years = 3

amount = principal * (1 + rate) ** years

print(f'Final Amount: {amount:.2f}')
```

---

## 📊 Part 12: Calculating Percentage

Formula:

```text
Percentage = (Obtained / Total) × 100
```
Python:
```python
obtained = 425
total = 500

percentage = (obtained / total) * 100

print(f'Percentage: {percentage:.2f}%')
# 85.00%
```
---
## 🎯 Part 13: Today's Practice Task

Create a Python program that:

1. Calculates the area of a circle.
2. Calculates compound interest.
3. Calculates a percentage.
4. Displays all results using f-strings.
5. Uses two decimal places where needed.

Example:

```python
print(f'Circle Area: {area:.2f}')
print(f'Final Amount: {amount:.2f}')
print(f'Percentage: {percentage:.2f}%')
```

---

## 📋 Part 14: Quick Reference

| Concept             | Meaning             |
| ------------------- | ------------------- |
| `/`                 | True division       |
| `//`                | Floor division      |
| `%`                 | Remainder           |
| `**`                | Exponent            |
| `+=`                | Add and assign      |
| `-=`                | Subtract and assign |
| `*=`                | Multiply and assign |
| `/=`                | Divide and assign   |
| `PEMDAS`            | Order of operations |
| `ZeroDivisionError` | Division by zero    |

---
## 🔄 Part 15: Day 5 vs Day 6
**Day 5:**
> What type of value am I working with?
**Day 6:**
> What can I calculate with these values?
Day 5 introduced data types.
Day 6 uses numbers to perform calculations.
---
## ❓ Part 16: Frequently Asked Questions

**Q: Why does `10 / 2` give `5.0`?**
Because `/` always performs true division and returns a float.
**Q: What is the difference between `/` and `//`?**
`/` gives the precise decimal result, while `//` performs floor division.
**Q: What does `%` do?**
It returns the remainder after division.
**Q: Which operator is used for powers?**
`**`
**Q: What happens when I divide by zero?**
Python raises a `ZeroDivisionError`.
---
## 🎓 Key Takeaways
1. ✅ Python uses `int` and `float` for numbers.
2. ✅ Python has seven main arithmetic operators.
3. ✅ `/` gives a float; `//` performs floor division.
4. ✅ `%` gives the remainder.
5. ✅ `**` calculates powers.
6. ✅ Python follows PEMDAS.
7. ✅ Shorthand operators simplify variable updates.
8. ✅ Parentheses make calculations clear.
9. ✅ Real-world formulas can be written directly in Python.
10. ✅ Arithmetic is an important foundation for future programming and data analysis.

---
**Ready for Day 7?**
Next: **Week 1 Review — Building a Complete Student Profile Program!** 🚀
