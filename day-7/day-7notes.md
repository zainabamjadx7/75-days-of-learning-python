# Day 7: Week 1 Review — Student Profile Program 🐍

**Date**: Day 7 / 75 | **Difficulty**: ⭐ Beginner | **Time**: 30 mins

---

## 🎯 What You'll Learn Today

* Review Days 1–6
* Combine variables, data types, and arithmetic
* Use f-strings for formatted output
* Calculate total marks, percentage, and average
* Build a complete Student Profile program
* Identify common mistakes

---

## 📚 Part 1: Week 1 Skill Map

| Day       | Main Topic                                      |
| --------- | ----------------------------------------------- |
| **Day 1** | Python & VS Code setup                          |
| **Day 2** | `print()`, strings, quotes                      |
| **Day 3** | `sep`, `end`, f-strings, `:.2f`                 |
| **Day 4** | Variables, assignment, `snake_case`             |
| **Day 5** | `str`, `int`, `float`, `bool`, `None`, `type()` |
| **Day 6** | Arithmetic operators & formulas                 |

Today's project combines all these concepts.

---

## 💻 Part 2: Quick Environment Check

Create a new file:

```text
week1_review.py
```

Test your Python setup:

```python
print('Week 1 review starting')
```

Run it using the VS Code Run button or terminal.

---

## 📝 Part 3: Quick `print()` & f-String Review

### Custom Separator

```python
print('a', 'b', sep='-')
# a-b
```

### f-String

```python
name = 'Zainab'
print(f'Name: {name}')
```

### Decimal Formatting

```python
gpa = 3.756
print(f'GPA: {gpa:.2f}')
# GPA: 3.76
```

---

## 🔤 Part 4: Variables Review

Use clear `snake_case` names.

```python
student_name = 'Zainab'
subject_1_marks = 78

print(subject_1_marks)

subject_1_marks = 82
print(subject_1_marks)
```

Remember: **Create a variable before using it.**

---

## 🔢 Part 5: Data Types Review

Use `type()` to check a value's type.

```python
print(type(student_name))
# str

print(type(subject_1_marks))
# int
```

When division is used for percentage or average, the result becomes a `float`.

---

## 🧮 Part 6: Arithmetic Review

### Total Marks

```python
total_marks = m1 + m2 + m3 + m4 + m5
```

### Percentage

```python
percentage = (total_marks / max_total_marks) * 100
```

### Average

```python
average = total_marks / 5
```

Parentheses make the percentage calculation clear.

---

## 🧩 Part 7: Designing the Student Profile

### Program Plan

1. Store student's name.
2. Store marks for 5 subjects.
3. Calculate total marks.
4. Calculate percentage.
5. Calculate average.
6. Display everything using f-strings.

Planning before coding makes larger programs easier to build.

---

## 📦 Part 8: Step 1 — Store the Data

```python
student_name = 'Zainab'

subject_1_marks = 78
subject_2_marks = 85
subject_3_marks = 90
subject_4_marks = 74
subject_5_marks = 88

max_marks_per_subject = 100
```

---

## 🧮 Part 9: Step 2 — Calculate Results

```python
total_marks = (
    subject_1_marks +
    subject_2_marks +
    subject_3_marks +
    subject_4_marks +
    subject_5_marks
)

max_total_marks = max_marks_per_subject * 5

percentage = (total_marks / max_total_marks) * 100

average = total_marks / 5
```

---

## 🎨 Part 10: Step 3 — Display a Formatted Card

```python
print('=' * 30)
print(f'STUDENT PROFILE: {student_name}')
print('=' * 30)

print(f'Subject 1: {subject_1_marks}')
print(f'Subject 2: {subject_2_marks}')
print(f'Subject 3: {subject_3_marks}')
print(f'Subject 4: {subject_4_marks}')
print(f'Subject 5: {subject_5_marks}')

print('-' * 30)
print(f'Total Marks: {total_marks}')
print(f'Percentage: {percentage:.2f}%')
print(f'Average: {average:.2f}')

print('=' * 30)
```

---

## 🔍 Part 11: Common Review-Day Mistakes & Fixes

### ❌ 1. Checking Notes Too Early

Review means trying to remember first, then checking notes if you're stuck.

**Fix:** Try rebuilding the program from memory before looking at the solution.

---

### ❌ 2. Forgetting Parentheses in Percentage

```python
percentage = total_marks / max_total_marks * 100
```

This works, but parentheses make the intention clearer.

**Better:**

```python
percentage = (total_marks / max_total_marks) * 100
```

---

### ❌ 3. Mixing Up `total_marks` and `max_total_marks`

* `total_marks` → Marks actually obtained
* `max_total_marks` → Maximum possible marks

Swapping them can produce an incorrect percentage.

---

### ❌ 4. Forgetting `:.2f`

Without formatting, decimals may display with unnecessary digits.

**Better:**

```python
print(f'Percentage: {percentage:.2f}%')
print(f'Average: {average:.2f}')
```

---

## 🎯 Part 12: Today's Practice Task

Build the complete **Student Profile Program**.

### Requirements

* Store your name.
* Store marks for 5 subjects.
* Store maximum marks per subject.
* Calculate total marks.
* Calculate percentage.
* Calculate average.
* Display a formatted profile card.
* Use `:.2f` for percentage and average.
* Use divider lines such as `'=' * 30`.
* Save and run the program.

### 💡 Challenge

Try building the complete program **without looking at the notes first**.

---

## 📋 Part 13: Week 1 Quick Reference

| Concept      | What You Learned        |
| ------------ | ----------------------- |
| `print()`    | Display output          |
| `sep`        | Change separator        |
| `end`        | Change ending           |
| f-string     | Insert values into text |
| `:.2f`       | 2 decimal places        |
| Variable     | Store a value           |
| `snake_case` | Variable naming style   |
| `type()`     | Check data type         |
| `+`          | Addition                |
| `/`          | Division                |
| `*`          | Multiplication          |
| `**`         | Exponent                |

---

## ❓ Part 14: Frequently Asked Questions

**Q: What if I can't remember a Day 1–6 concept?**
Review that specific day's notes, practise the small example, and try again.

**Q: Does my program need to look exactly like the example?**
No. Variable names, labels, and formatting can be different as long as the required concepts work correctly.

**Q: Does my program have to be the same length?**
No. A shorter or longer program is fine if it correctly stores, calculates, and displays the required information.

**Q: What comes after Week 1?**
Day 8 starts Week 2 and introduces **user input**, allowing programs to receive information from the person running them.

---

## 🎓 Key Takeaways

1. ✅ Day 7 reviews everything from Days 1–6.
2. ✅ Variables store student information.
3. ✅ Arithmetic calculates totals, percentages, and averages.
4. ✅ f-strings create clean formatted output.
5. ✅ `:.2f` keeps decimal results readable.
6. ✅ Planning before coding makes programs easier to build.
7. ✅ The Student Profile Program combines the main skills from Week 1.

---

**🎉 Week 1 Complete!**

**Ready for Day 8?**
Next: **Python User Input — Making Programs Interactive!** 🚀
