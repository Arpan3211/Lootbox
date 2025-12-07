

# ** Python Notes (FULL Detailed Notes)**

---

## **1. What is a Variable?**

A **variable** is a container used to store data in Python.
It acts like a name tagged to a value.

In simple words:
**Variable = Name that stores some data (value)**

Example:

```python
x = 10
name = "Arpan"
```

---

## **2. Why Do We Use Variables?**

* To store data
* To reuse values
* To perform calculations
* To make programs dynamic

Example:

```python
radius = 7
area = 3.14 * radius * radius
```

---

## **3. Rules for Naming Variables**

Python has strict naming rules:

### ** Valid Rules**

* Can contain **letters (a–z/A–Z)**, **digits (0–9)**, and **underscore (_)**
* Must **start with a letter or underscore**
* Cannot start with a number
* Case-sensitive (`age`, `Age`, `AGE` are different)
* Cannot use Python keywords (e.g., `for`, `if`, `class`, etc.)

### ** Examples**

Valid:

```python
name = "Arpan"
age_22 = 22
_total = 500
```

Invalid:

```python
2name = "Arpan"     # starts with number
my-name = "a"       # hyphen not allowed
class = 10          # keyword not allowed
```

---

## **4. Variable Declaration**

Python does **not** require explicit type declaration.

Example:

```python
x = 5
x = "Hello"     # type can change → Python is dynamically typed
```

---

## **5. Dynamically Typed Language**

Python automatically detects the type of variable based on assigned value.

Example:

```python
a = 10        # int  
a = 10.5      # float  
a = "Python"  # string
```

This is called **Dynamic Typing**.

---

## **6. Assigning Values to Variables**

Python allows:

### ** Single Assignment**

```python
x = 100
```

### ** Multiple Assignment**

Assign multiple variables at the same time:

```python
a, b, c = 10, 20, 30
```

### ** Same Value to Multiple Variables**

```python
x = y = z = 5
```

---

## **7. Types of Variables**

### **(A) Local Variable**

Defined **inside a function**, used only inside that function.

```python
def test():
    x = 10   # local variable
    print(x)
```

### **(B) Global Variable**

Declared **outside** any function, accessible everywhere.

```python
x = 100  # global variable

def show():
    print(x)
```

#### Use `global` keyword to modify global variable inside a function:

```python
count = 0

def update():
    global count
    count += 1
```

---

## **8. Constants**

Python doesn’t have true constants,
but by convention **uppercase names** are used for constant-like values.

Example:

```python
PI = 3.14
MAX_SIZE = 100
```

---

## **9. Memory Management & Variables**

When you assign a variable:

```python
a = 10
b = a
```

* `10` is stored in memory
* `a` and `b` both point to the same memory location
* Python uses **reference model**, not copying every time

---

## **10. Variable Type Checking**

To check the type of a variable:

```python
x = 10
print(type(x))
```

Output:

```
<class 'int'>
```

---

## **11. Input and Variables**

Taking user input:

```python
name = input("Enter your name: ")
age = int(input("Enter age: "))
```

`input()` always returns a **string**, so convert when needed.

---

## **12. Best Practices for Naming Variables**

* Use meaningful names:

  * `age`, `username`, `price`, `total_amount`
* Use snake_case:

  * `first_name`, `total_marks`
* Avoid short names except loop counters:

  * `i`, `j`, `k` are okay for loops
* Avoid confusing names:

  * `l`, `I`, `O` (look like numbers)

---

# ** Summary (Quick Revision)**

| Topic               | Explanation                                           |
| ------------------- | ----------------------------------------------------- |
| Variable            | Name used to store data                               |
| Dynamic Typing      | Type determined at runtime                            |
| Naming Rules        | cannot start with number, case-sensitive, no keywords |
| Multiple assignment | `a, b = 1, 2`                                         |
| Global vs Local     | scope defines accessibility                           |
| Constants           | use uppercase names                                   |
| Type check          | `type()`                                              |


------------------------------------------------------------------------------------------------------------------

# **Python Type Casting**

Type casting means **converting one data type into another**.
Python has two types of casting:

1. **Implicit Type Casting (Automatic)**
2. **Explicit Type Casting (Manual)**

Let’s understand both with examples.

---

# **Implicit Type Casting (Automatic Casting)**

Python automatically converts one data type to another **without losing data**.

✔ Happens when:

* A smaller type converts into a larger type
* No data loss occurs

### Example: int → float

```python
num_int = 10
num_float = 10.5

result = num_int + num_float
print(result)        # 20.5
print(type(result))  # <class 'float'>
```

Python automatically converted `num_int (int)` into a `float` while adding.

---

# **Explicit Type Casting (Manual Casting)**

You manually convert one data type into another using type functions.

Python provides these casting functions:

| Function  | Converts To           |
| --------- | --------------------- |
| `int()`   | Integer               |
| `float()` | Floating-point number |
| `str()`   | String                |
| `bool()`  | Boolean               |
| `list()`  | List                  |
| `tuple()` | Tuple                 |
| `set()`   | Set                   |
| `dict()`  | Dictionary            |

Let’s see each one clearly.

---

# **int() – Convert to Integer**

Removes decimal values and returns only the whole number.

```python
x = int(10.8)     # 10
y = int("25")     # 25
```

 **Not allowed**

```python
int("hello")   # Error
int("10.55")   # Error (string with decimal)
```

---

# **float() – Convert to Float**

```python
a = float(5)        # 5.0
b = float("12")     # 12.0
c = float("10.55")  # 10.55
```

---

# **str() – Convert to String**

Anything can be converted to string.

```python
str(10)        # "10"
str(10.5)      # "10.5"
str(True)      # "True"
```

---

# **bool() – Convert to Boolean**

| Value                                | Result  |
| ------------------------------------ | ------- |
| `0`, `0.0`, `""`, `[]`, `{}`, `None` | `False` |
| Any other value                      | `True`  |

```python
bool(0)        # False
bool(10)       # True
bool("")       # False
bool("hello")  # True
```

---

# 🔹 **list(), tuple(), set() – Convert Between Collections**

```python
list("hello")      # ['h', 'e', 'l', 'l', 'o']
tuple([1, 2, 3])   # (1, 2, 3)
set([1, 2, 2, 3])  # {1, 2, 3}
```

---

# 🔹 **dict() – Convert to Dictionary**

Only works if data is in **key–value** pairs:

```python
dict([("a", 1), ("b", 2)])  
# {'a': 1, 'b': 2}
```

---

# **Important Notes**

### 1. Type casting can cause **data loss**

```python
int(10.99)  # 10 (decimal removed)
```

### 2. Strings must be in a **valid format**

```python
int("10")     # OK
int("10a")    # Error
```

### 3. Implicit casting **never loses data**, explicit casting **may lose data**

---

# **Real-Life Example**

### Total price calculation

```python
price = "150"
tax = 18.5

total = int(price) + tax
print(total)   # 168.5
```

---

# Summary Table

| Type         | Description                                         |
| ------------ | --------------------------------------------------- |
| **Implicit** | Python converts automatically (safe conversion)     |
| **Explicit** | Developer converts manually using casting functions |

---

