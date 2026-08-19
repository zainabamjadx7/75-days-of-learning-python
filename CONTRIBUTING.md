# Contributing to 75 Days of Learning Python 🚀

First off, **thank you** for considering contributing! This project welcomes contributions from everyone, regardless of skill level.

---

## 📝 Code of Conduct

Be respectful, supportive, and inclusive. We're all here to learn!

- 🤝 Help others learn
- ✨ Celebrate all contributions
- 🙅 No harassment or discrimination
- 💭 Constructive feedback only

---

## 🎯 Ways to Contribute

### 1️⃣ Solve Unsolved Tasks

Many days have tasks waiting for solutions!

**Steps:**
1. Browse `/days` folder
2. Find a `day-XX-tasks.md` without a `day-XX-solution.py`
3. Solve the problem
4. Create a file: `day-XX-solution.py`
5. Add comments explaining your approach
6. Submit a Pull Request

**Example PR title:** `Add solution for Day 5`

---

### 2️⃣ Improve Explanations

- Concept unclear? Rewrite it simpler!
- Add more examples to notes
- Explain why a solution works
- Create visual diagrams

**Steps:**
1. Edit the `day-XX-notes.md` file
2. Make it clearer/more detailed
3. Commit with message: `Improve Day X explanation`
4. Submit PR

---

### 3️⃣ Add Alternative Solutions

Different approach to a problem? Awesome!

**Steps:**
1. Create: `day-XX-solution-alternative.py`
2. Add a comment explaining your approach
3. List pros/cons vs. the main solution
4. Submit PR with title: `Add alternative solution for Day X`

**Example:**
```python
# Alternative Solution for Day 5
# Approach: Using list comprehension instead of for loop
# Pros: More Pythonic, faster
# Cons: Less readable for beginners

numbers = [1, 2, 3, 4, 5]
squared = [x**2 for x in numbers]
print(squared)
```

---

### 4️⃣ Report Issues

Found a bug? Typo? Incorrect output?

**Steps:**
1. Check if issue already exists
2. Click "Issues" tab on GitHub
3. Click "New Issue"
4. Describe the problem clearly

**What to include:**
- What's the problem?
- Which file/day is affected?
- Expected vs. actual behavior
- Screenshots if helpful

---

### 5️⃣ Improve Documentation

- Fix typos in README or other files
- Add more resources/links
- Create cheat sheets
- Write learning tips

---

## 🔧 Getting Started with Git & GitHub

### First Time? No Problem!

1. **Install Git** - [Download](https://git-scm.com/)
2. **Create GitHub Account** - [Join](https://github.com/join)
3. **Learn basics** - [GitHub Hello World](https://guides.github.com/activities/hello-world/)

### Step-by-Step PR Process

#### Step 1: Fork the Repository
Click the **"Fork"** button (top-right of this repo)

#### Step 2: Clone Your Fork
```bash
git clone https://github.com/YOUR-USERNAME/75-days-of-learning-python.git
cd 75-days-of-learning-python
```

#### Step 3: Create a New Branch
```bash
git checkout -b add-day-5-solution
```

**Branch naming tips:**
- `add-day-XX-solution` - Adding a solution
- `fix-day-XX-typo` - Fixing typos
- `improve-day-XX-explanation` - Better explanation
- `add-alternative-day-XX` - Alternative solution

#### Step 4: Make Your Changes

Edit files as needed. Examples:

**Adding a solution:**
```bash
cp day-05-solution.py  # Copy from template
# Edit day-05-solution.py with your solution
```

**Improving notes:**
```bash
# Edit day-05-notes.md in your favorite editor
```

#### Step 5: Commit Your Changes
```bash
# Check what changed
git status

# Add your changes
git add .

# Commit with a clear message
git commit -m "Add solution for Day 5 with explanation"
```

**Commit message tips:**
- Start with action verb: Add, Fix, Improve, Remove
- Be specific: What did you change?
- Keep it under 50 characters
- Good: `Add Day 5 solution for loop exercise`
- Bad: `fixed stuff`

#### Step 6: Push to GitHub
```bash
git push origin add-day-5-solution
```

#### Step 7: Create a Pull Request
1. Go to your fork on GitHub
2. Click **"Compare & pull request"** (green button)
3. Write a clear title and description:
   - **Title**: `Add solution for Day 5`
   - **Description**: 
     ```
     This PR adds a complete solution for Day 5 tasks.
     
     - Solves Task 1: String concatenation
     - Solves Task 2: List manipulation
     - All outputs tested and working
     
     Difficulty: Medium
     ```
4. Click **"Create Pull Request"**

#### Step 8: Respond to Reviews
- I'll review your PR
- May ask for changes
- Update your branch if needed:
  ```bash
  git add .
  git commit -m "Address review feedback"
  git push
  ```

---

## ✅ Contribution Checklist

Before submitting a PR, make sure:

- [ ] Code follows Python best practices
- [ ] Comments explain the solution
- [ ] No syntax errors (test before submitting!)
- [ ] Files are named correctly
- [ ] Commit message is clear
- [ ] No unnecessary files added
- [ ] You've tested your code

---

## 🐍 Python Style Guide

Keep code clean and readable!

### Good Practices:
```python
# ✅ Good - Clear and readable
def calculate_sum(numbers):
    """Calculate sum of numbers in a list."""
    total = 0
    for num in numbers:
        total += num
    return total

# ✅ Good - Using built-in
result = sum(numbers)

# ❌ Bad - Unclear variable names
def cs(n):
    t = 0
    for x in n:
        t += x
    return t
```

### Naming Conventions:
```python
# Variables and functions: lowercase_with_underscores
user_name = "Zainab"
def calculate_total():
    pass

# Constants: UPPERCASE_WITH_UNDERSCORES
MAX_ATTEMPTS = 5

# Classes: PascalCase
class StudentProfile:
    pass
```

### Comments:
```python
# ✅ Good - Explains the why
# Skip even numbers because we only need odds
if num % 2 != 0:
    results.append(num)

# ❌ Bad - Obvious comment
x = 5  # Set x to 5
```

---

## 📚 Resource Files

These files help new contributors:

- `README.md` - Project overview
- `CONTRIBUTING.md` - This file
- `LICENSE` - Project license
- `.gitignore` - Files to ignore in Git
- `/resources/quick-reference.md` - Python cheatsheet

---

## ❓ Questions?

- Open an **Issue** with your question
- Email: zainabamjadali04@gmail.com
- Comment on existing issues/PRs
- Check existing discussions first

---

## 🎉 Your First Contribution

Don't know where to start?

1. Look for issues tagged `good-first-issue`
2. Pick a day without a solution
3. Solve the tasks and create a PR
4. That's it! You're a contributor now! 🎊

---

## 📖 Learn More About Git

- [Git Documentation](https://git-scm.com/doc)
- [GitHub Guides](https://guides.github.com/)
- [How to Write a Good Commit Message](https://chris.beams.io/posts/git-commit/)
- [Understanding Git Branches](https://www.atlassian.com/git/tutorials/using-branches)

---

## 🙏 Thank You!

Every contribution makes this project better. Whether it's code, docs, or ideas - **we appreciate you!**

Let's learn Python together! 🐍✨

---

**Happy Contributing!** 🚀

## Author
**Zainab Amjad**
