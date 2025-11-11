# 🐍 Python Reference Guide

A complete reference guide for Python beginners and juniors covering **Functional Programming**, **Data Management & Types**, and **Object-Oriented Programming (OOP)**.  
All sections are cleanly formatted for Markdown compatibility.

---

## 🧠 1. Functional Programming in Python

Functional programming focuses on using **functions as first-class citizens** and minimizing state changes.

### 🧩 Key Concepts

| Concept | Description |
|----------|--------------|
| **First-class functions** | Functions can be assigned to variables, passed as arguments, or returned. |
| **Pure functions** | Have no side effects; output depends only on input. |
| **Higher-order functions** | Take other functions as arguments or return them. |
| **Immutability** | Avoid changing objects in place. |
| **Recursion** | A function calls itself to solve a smaller problem. |

---

### ⚙️ Common Functional Tools

| Function / Concept | Description | Example |
|--------------------|--------------|----------|
| `map(func, iterable)` | Applies a function to each element. | `map(lambda x: x**2, [1,2,3]) → [1,4,9]` |
| `filter(func, iterable)` | Filters elements based on a condition. | `filter(lambda x: x%2==0, [1,2,3,4]) → [2,4]` |
| `reduce(func, iterable)` | Combines elements cumulatively. | `reduce(lambda a,b: a+b, [1,2,3]) → 6` |
| **List comprehension** | Pythonic concise way to create lists. | `[x**2 for x in [1,2,3,4]] → [1,4,9,16]` |
| **Lambda functions** | Anonymous, inline functions. | `(lambda a,b: a+b)(2,3) → 5` |

---

## 📊 2. Data Types and Data Management in Python

Understanding data types is essential for effective data manipulation and memory management.

---

### 🧱 Basic Data Types

| Type | Description | Example |
|------|--------------|----------|
| `int` | Integer numbers. | `42` |
| `float` | Decimal numbers. | `3.14` |
| `complex` | Complex numbers. | `2 + 3j` |
| `bool` | Boolean values. | `True` / `False` |
| `str` | Text strings. | `"Python"` |
| `NoneType` | Represents no value. | `None` |

---

### 🧩 Sequence Types

| Type | Description | Mutable | Example |
|------|--------------|----------|----------|
| `list` | Ordered collection. | ✅ Yes | `[1, 2, 3]` |
| `tuple` | Ordered and immutable. | ❌ No | `(10, 20)` |
| `range` | Sequence of numbers. | ❌ No | `range(0, 10)` |
| `str` | Sequence of characters. | ❌ No | `"Hello"` |

---

### 🗂️ Mapping & Set Types

| Type | Description | Mutable | Example |
|------|--------------|----------|----------|
| `dict` | Key-value pairs. | ✅ Yes | `{"name": "Josep"}` |
| `set` | Unordered unique elements. | ✅ Yes | `{1, 2, 3}` |
| `frozenset` | Immutable set. | ❌ No | `frozenset([1, 2, 3])` |

---

### 🔄 Type Conversion

| Function | Description | Example |
|-----------|--------------|----------|
| `int("10")` | String → Integer | `10` |
| `float("3.14")` | String → Float | `3.14` |
| `str(100)` | Number → String | `"100"` |
| `list("abc")` | String → List | `['a', 'b', 'c']` |
| `tuple([1, 2])` | List → Tuple | `(1, 2)` |
| `set([1, 1, 2])` | Remove duplicates | `{1, 2}` |

---

### 🧮 Mutable vs Immutable

| Category | Data Types |
|-----------|-------------|
| Mutable | `list`, `dict`, `set`, `bytearray` |
| Immutable | `int`, `float`, `tuple`, `str`, `frozenset`, `bytes` |

---

### ⚙️ Collections & Advanced Structures

| Structure | Description | Example |
|------------|--------------|----------|
| `namedtuple` | Tuple with named fields. | `Point = namedtuple("Point", "x y")` |
| `deque` | Double-ended queue (fast append/pop). | `deque([1,2,3])` |
| `Counter` | Counts element occurrences. | `Counter("banana") → {'a':3,'n':2,'b':1}` |
| `defaultdict` | Dict with default values. | `defaultdict(int)` |

---

### 🧰 DataFrames (pandas)

| Operation | Description | Example |
|------------|--------------|----------|
| `pd.DataFrame({...})` | Create a data frame. | `df = pd.DataFrame({"name":["Ana","Josep"],"age":[22,25]})` |
| `df.info()` | Overview of data types. | — |
| `df.describe()` | Summary statistics. | — |
| `df['col'].astype(type)` | Convert column type. | `df['age'] = df['age'].astype(int)` |
| `df.dropna()` | Remove missing values. | — |
| `df.fillna(value)` | Replace missing values. | — |

---

## 🏗️ 3. Object-Oriented Programming (OOP)

OOP models real-world entities as **objects** with attributes (data) and methods (behavior).

---

### 🧩 Classes & Objects

| Concept | Description |
|----------|--------------|
| **Class** | Blueprint for creating objects. |
| **Object** | Instance of a class. |

---

### 🧰 Attributes

| Type | Description |
|-------|--------------|
| **Instance attributes** | Unique to each object. |
| **Class attributes** | Shared among all instances. |

---

### ⚙️ Methods

| Type | Description |
|-------|--------------|
| **Instance methods** | Work on instance data (`self`). |
| **Class methods** | Work on class data (`@classmethod`). |
| **Static methods** | Utility functions not tied to instance or class. |

---

### 🧬 Encapsulation

| Concept | Description |
|----------|--------------|
| **Encapsulation** | Protects object data using private attributes (`_` or `__`). |
| **Accessors / Mutators** | Getters and setters to access or modify private attributes. |

---

### 🔗 Inheritance

| Concept | Description |
|----------|--------------|
| **Parent/Base class** | The original class being inherited from. |
| **Child/Derived class** | Inherits attributes and methods, can override them. |

---

### 🌀 Polymorphism

| Concept | Description |
|----------|--------------|
| **Polymorphism** | Same interface, different implementations. Example: `speak()` behaves differently for `Dog` and `Bird`. |

---

### ⚖️ Abstraction

| Concept | Description |
|----------|--------------|
| **Abstraction** | Hides complex details; achieved via abstract base classes (`ABC`) and abstract methods. |

---

### 🔄 Special Methods (Dunder Methods)

| Method | Description |
|---------|--------------|
| `__init__` | Constructor method. |
| `__str__` | Returns human-readable representation. |
| `__repr__` | Returns developer representation. |
| `__add__` | Defines behavior of `+` operator. |
| `__len__`, `__getitem__`, etc. | Customize built-in Python operations. |

---

## 🧾 Summary

| Topic | Key Concepts |
|--------|---------------|
| **Functional Programming** | Pure functions, `map`/`filter`/`reduce`, lambda, immutability. |
| **Data Management** | Built-in types, sequences, mappings, sets, mutability, conversions, pandas. |
| **OOP** | Classes, objects, attributes, methods, encapsulation, inheritance, polymorphism, abstraction. |

---

👨‍💻 **Author:** Josep  
📚 **Purpose:** Master reference for Python fundamentals in a single Markdown file.