# 🐍 Basic Python– Study Summary

## ✅ Overview

- **Readable language**
- **Used for:**
  - **Web** → Python + Django
  - **System tasks** → automate repetitive work
  - **Data Science** → `pandas`, `numpy`, `scikit-learn`, `keras`, `tensorflow`, `pytorch`
  - **AI** → stable, flexible, many tools
- **Indentation** controls code blocks (instead of `{}` like in JS)

---

## 🔤 Python Basics

### 🗨️ Comments & Strings

- `#` → single-line comment
- `''' '''` or `` → multi-line comment
- Strings: `'text'`, `"text"`, `'''text'''`

### 🧪 Install Python Version

```bash
pyenv install 3.x.x
pyenv global 3.x.x
```

Or use alias:

```bash
alias python3='python3.13'
python3 --version
```

### 🧮 Variables

- Must start with a **letter or `_`**
- No spaces, use English
- Use short, clear names

#### f-Strings and Format

```python
f"Hello, my name is {name}"
"Hello, {}".format(name)
```

---

## 🧱 Data Types

### 🔢 Numbers

- **Integers**: 1, -3, 0
- **Floats**: 2.5, -0.1

### 📦 List

```python
my_list[1]         # Access
my_list[:2]        # Slice
my_list * 3        # Repeat
my_list.append(x)  # Add
x.extend(y)        # Merge
x + y              # Combine
```

### 📊 Set

```python
a = {1, 2, 3}
a.add(4)
a.union(b)
a.intersection(b)
a.difference(b)
```

| Use Case                   | Type |
| -------------------------- | ---- |
| Order + Duplicates         | List |
| No duplicates, fast lookup | Set  |

### 🔒 Tuple

```python
t = (1, 2, 3)
list(t)  # convert to list to edit
```

### 🔑 Dictionary

```python
person = {"name": "Choti", "age": 30}
person["name"]       # access
person["city"] = "Antwerp"  # add
del person["city"]          # delete
person.pop("city")
person.clear()              # clear all
```

---

## ➗ Arithmetic Operators

| Operator  | Use                 |
| --------- | ------------------- |
| `+ - * /` | Basic math          |
| `//`      | Floor division      |
| `%`       | Modulus (remainder) |
| `**`      | Exponentiation      |

- `/` returns float
- `//` returns integer
- `:.2f` → 2 decimal places formatting

```python
f"Total: {price:.2f}"
```

---

## 🔁 Conditions & Loops

### 🚦 Conditionals

```python
if condition:
elif another:
else:
```

### 🔗 Logical Operators

- `and`, `or`, `not`

### 🔄 Loops

```python
for i in range(5):
while condition:
```

- `break` → stop loop
- `continue` → skip rest of loop, go to next

### ⏱️ Range

```python
range(start, stop, step)
range(1, 6)  # 1 to 5
```

### 🔄 Reverse

```python
list.reverse()  # in-place, returns None
list[::-1]      # reversed copy
```

---

## 🧰 Extra Tools

### 🔁 Flatten List

```python
flat = [item for sublist in list_of_lists for item in sublist]
```

### 🧮 Eval Function

```python
eval("2 + 2")  # → 4
```

### 🧩 Unpack Dictionary

```python
def show(**kwargs):
    for k, v in kwargs.items():
        print(k, v)

show(name="Choti", age=30)
```

### 🔢 Dict with Index

```python
for i, (k, v) in enumerate(my_dict.items()):
    print(f"{i}: {k} = {v}")
```

### 🔧 Dict from Lists

```python
keys = ("brand", "model")
values = ("Ford", "Mustang")
car = {k: v for k, v in zip(keys, values)}
```

---

## 🧼 String & List Methods

```python
x = txt.split("#")       # split string to list
x = "#".join(listname)   # join list to string
```
