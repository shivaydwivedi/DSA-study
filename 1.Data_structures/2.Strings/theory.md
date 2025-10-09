

# **Strings in Python**

A **string** is a collection of characters enclosed in quotes.
These characters can be letters, digits, symbols, or whitespace.

---

## **1. Creating Strings**

Strings can be created in multiple ways:

* **Single quotes:**

  ```python
  s = 'hello'
  ```
* **Double quotes:**

  ```python
  s = "hello"
  ```
* **Triple quotes (for multiline strings):**

  ```python
  s = '''This is
  a multiline
  string.'''
  ```

---

## **2. Accessing String Elements**

* Strings are **index-based**; indexing starts at **0**.

  ```python
  s = "hello"
  print(s[0])   # h
  print(s[-1])  # o
  ```
* **Slicing:** Used to extract a substring.

  ```python
  s[1:4]    # 'ell'
  s[::-1]   # 'olleh' (reversing)
  ```
* Accessing an index **out of range** raises an **IndexError**.

---

## **3. Iterating Over Strings**

Strings are **iterable**, so you can loop through each character:

```python
for ch in "hello":
    print(ch)
```

---

## **4. Immutability**

* Strings in Python are **immutable** — you cannot change them directly.
* However, you can **create a modified version** using operations like concatenation, slicing, or `replace()`.

Example:

```python
s = 'shivay'
s = 'S' + s[1:]
print(s)  # Shivay
```

---

## **5. Deleting a String**

* You can delete a string variable using `del`.

  ```python
  s = "hello"
  del s
  ```
* Accessing it afterward raises a **NameError** because the variable no longer exists.

---

## **6. Updating Strings**

Since strings are immutable, “updating” creates a new string.

Example:

```python
s = "hello"
s = s.replace("h", "H")
print(s)  # Hello
```

---

## **7. Common String Methods**

| Method          | Description                       | Example                                   |
| --------------- | --------------------------------- | ----------------------------------------- |
| `len(s)`        | Returns length                    | `len("hello") → 5`                        |
| `upper()`       | Converts to uppercase             | `"abc".upper() → "ABC"`                   |
| `lower()`       | Converts to lowercase             | `"Hi".lower() → "hi"`                     |
| `strip()`       | Removes leading/trailing spaces   | `"  hi  ".strip() → "hi"`                 |
| `find(sub)`     | Returns index of first occurrence | `"hello".find("e") → 1`                   |
| `replace(a, b)` | Replaces substring                | `"abc".replace("a", "x") → "xbc"`         |
| `title()`       | Capitalizes each word             | `"good morning".title() → "Good Morning"` |
| `swapcase()`    | Swaps uppercase ↔ lowercase       | `"Hi".swapcase() → "hI"`                  |

---

## **8. String Formatting**

1. **f-strings (Recommended):**

   ```python
   name = "Shivay"
   print(f"Hello, {name}!")
   ```

2. **Using `format()`:**

   ```python
   print("Hello, {}".format(name))
   ```

---

## **9. Membership Testing**

Use the `in` keyword to check for substring presence:

```python
"py" in "python"      # True
"java" in "python"    # False
```

---

## **Practice Problems**

### **1. Repeat the Strings**

**Problem:**
Given two strings `a` and `b`, form a new string as `shorter + longer + shorter`.
(Guaranteed that lengths differ.)

**Example:**

```
Input:  a = "Hi", b = "There"
Output: "HiThereHi"
```

---

### **2. String Functions I**

**Task:**
Implement various string operations: `title()`, `swapcase()`, `find()`, `strip()`.

**Example:**

```
Input:
str = "hello"
x = "llo"
Output:
hello
2
Hello
HELLO
```

---

### **3. Convert String to Lowercase**

**Problem:** Convert all uppercase letters in a string to lowercase.

**Example:**

```
Input:  s = "ABCddE"
Output: "abcdde"
```

---

### **4. Remove Duplicate Characters**

**Problem:**
Remove all duplicate characters while maintaining order.

**Example:**

```
Input:  s = "geEksforGEeks"
Output: "geEksforG"
```

---

### **5. Check Palindrome**

**Problem:**
Check whether a given string reads the same backward and forward (case-insensitive).

**Example:**

```
Input:  s = "TenEt"
Output: True
```

---

## **Summary**

* Strings are **immutable**, **indexed**, and **iterable**.
* Common operations: slicing, concatenation, and built-in methods.
* Use **f-strings** for modern and readable formatting.
* When you need to modify a string → always create a **new** one.
* Useful for textual data, pattern matching, and data processing.


