
# 🧠 Functional Programming in Python

Functional programming focuses on writing code using **pure functions**, **immutability**, and **expressions**, instead of side effects or imperative steps.

---

## ⚙️ Core Concepts

| Concept | Description | Example |
|----------|--------------|----------|
| **Pure Function** | Returns the same result for the same input, no side effects. | ```python\ndef add(a, b):\n    return a + b``` |
| **Immutability** | Data isn’t modified; new values are created instead. | ```python\nx = [1, 2, 3]\ny = x + [4]``` |
| **Expression vs Statement** | Expressions produce a value; statements perform an action. | `x = 2 + 3` (expression) |
| **First-Class Functions** | Functions can be stored, passed, and returned like data. | ```python\nf = print\nf("Hi")``` |
| **Higher-Order Functions** | Accept or return other functions. | ```python\nmap(func, iterable)``` |

---

## 🧮 Built-in Functional Tools

| Function | Description | Example |
|-----------|--------------|----------|
| `map(func, iterable)` | Apply a function to each element. | ```python\nlist(map(lambda x: x*2, [1,2,3]))``` |
| `filter(func, iterable)` | Keep only elements that satisfy a condition. | ```python\nlist(filter(lambda x: x>2, [1,2,3,4]))``` |
| `reduce(func, iterable)` | Combine elements into a single value. | ```python\nfrom functools import reduce\nreduce(lambda a,b: a+b, [1,2,3])``` |
| `zip()` | Combine multiple iterables. | ```python\nlist(zip(['a','b'], [1,2]))``` |
| `enumerate()` | Iterate with index and value. | ```python\nlist(enumerate(['a','b','c']))``` |

---

## 🧰 Lambda Functions

Small anonymous functions.  
```python
double = lambda x: x * 2
print(double(5))  # 10