# 🧠 Programación Funcional en Python

La **programación funcional** se basa en escribir código usando **funciones puras**, **inmutabilidad** y **expresiones**, en lugar de estructuras imperativas.

---

## ⚙️ Conceptos Clave

| Concepto | Descripción | Ejemplo |
|-----------|--------------|----------|
| **Función pura** | No tiene efectos secundarios ni depende de variables externas. | ```python def suma(a, b): return a + b``` |
| **Inmutabilidad** | Los datos no cambian; se crean nuevos valores. | ```python x = [1, 2, 3]; y = x + [4]``` |
| **Expresiones vs. Sentencias** | Expresiones devuelven valor; sentencias ejecutan acciones. | `x = 2 + 3` (expresión) |
| **Primera clase** | Las funciones se pueden guardar en variables o pasar como argumentos. | ```python f = print; f("Hola")``` |
| **Alta orden** | Funciones que reciben o devuelven otras funciones. | ```python map(func, iterable)``` |

---

## 🧮 Funciones Funcionales Integradas

| Función | Descripción | Ejemplo |
|----------|--------------|----------|
| `map(func, iterable)` | Aplica una función a cada elemento. | ```python list(map(lambda x: x*2, [1,2,3]))``` |
| `filter(func, iterable)` | Filtra elementos según una condición. | ```python list(filter(lambda x: x>2, [1,2,3,4]))``` |
| `reduce(func, iterable)` | Reduce una lista a un valor (requiere `from functools import reduce`). | ```python reduce(lambda a,b: a+b, [1,2,3])``` |
| `zip()` | Une listas por posición. | ```python list(zip(['a','b'], [1,2]))``` |
| `enumerate()` | Devuelve índice y valor. | ```python list(enumerate(['a','b','c']))``` |

---

## 🧰 Funciones Lambda (Anónimas)

Pequeñas funciones sin nombre.  
```python
doble = lambda x: x * 2
print(doble(5))  # 10
