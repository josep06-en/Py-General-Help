# 📘 Python & Version Control Reference Guide

Welcome to the **Python & Git Command Reference** — a complete knowledge base designed for **junior developers** who want to strengthen their foundations in:

- ⚙️ Command Line (CMD) Basics  
- 🌀 Git Version Control  
- 🧠 Functional Programming in Python  
- 📊 Data Types & Data Management  
- 🏗️ Object-Oriented Programming (OOP)

This guide is written in Markdown for clarity and can be opened directly in **VS Code** or **GitHub**.

---

## 🗂️ Table of Contents

1. [⚙️ CMD & Git Commands](#️-cmd--git-commands)
2. [🧠 Functional Programming in Python](#-functional-programming-in-python)
3. [📊 Data Types & Data Management in Python](#-data-types--data-management-in-python)
4. [🏗️ Object-Oriented Programming (OOP) in Python](#-object-oriented-programming-oop-in-python)
5. [📎 Author & Credits](#-author--credits)

---

## ⚙️ CMD & Git Commands

### 🖥️ Command Line (CMD)

| Command | Description | Example |
|----------|-------------|----------|
| `dir` | List files and folders in current directory | `dir` |
| `cd` | Change directory | `cd Desktop` |
| `cls` | Clear the screen | `cls` |
| `mkdir` | Create a folder | `mkdir project` |
| `rmdir` | Delete an empty folder | `rmdir test` |
| `del` | Delete files | `del file.txt` |
| `copy` | Copy files | `copy a.txt b.txt` |
| `move` | Move or rename files | `move a.txt newfolder\` |
| `exit` | Close the terminal | `exit` |

### 🌀 Git Commands

| Command | Description | Example |
|----------|-------------|----------|
| `git init` | Initialize a Git repository | `git init` |
| `git clone <url>` | Clone a repository | `git clone https://github.com/user/repo.git` |
| `git status` | Check current changes | `git status` |
| `git add <file>` | Stage a file for commit | `git add main.py` |
| `git commit -m "msg"` | Commit staged files | `git commit -m "Initial commit"` |
| `git log` | Show commit history | `git log` |
| `git diff` | Show file changes | `git diff` |
| `git branch` | List branches | `git branch` |
| `git checkout -b <branch>` | Create and switch branch | `git checkout -b dev` |
| `git merge <branch>` | Merge a branch | `git merge dev` |
| `git pull` | Fetch + merge remote changes | `git pull` |
| `git push` | Upload commits to remote | `git push origin main` |
| `git remote -v` | Show remotes | `git remote -v` |
| `git reset --hard <commit>` | Reset to a previous commit | `git reset --hard a1b2c3` |
| `git revert <commit>` | Undo a specific commit | `git revert 4f5g6h` |

---

## 🧠 Functional Programming in Python

Functional programming is a **declarative style** that focuses on *what* to do, not *how* to do it.

Key principles:
- Use **pure functions**
- Avoid **mutating state**
- Rely on **higher-order functions** (`map`, `filter`, `reduce`)

```python
from functools import reduce

nums = [1, 2, 3, 4]
squared = list(map(lambda x: x**2, nums))
evens = list(filter(lambda x: x % 2 == 0, nums))
total = reduce(lambda a, b: a + b, nums)
print(squared, evens, total)
