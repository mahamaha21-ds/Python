# Python Fundamentals: List, Tuple, Set, Dictionary

## Basic Terms

### Mutable

Can be changed after creation.

Example:

```python
numbers = [1, 2, 3]
numbers.append(4)
```

### Immutable

Cannot be changed after creation.

Example:

```python
colors = ("Red", "Green", "Blue")
```

---

### Ordered

Items keep their position.

Example:

```python
["Apple", "Banana", "Orange"]
```

Apple is always at index 0.

### Unordered

Items do not have a fixed position.

Example:

```python
{"Apple", "Banana", "Orange"}
```

The order may change when displayed.

---

# Quick Comparison

| Type       | Symbol      | Position Maintained | Can Modify | Duplicate Values      |
| ---------- | ----------- | ------------------- | ---------- | --------------------- |
| List       | []          | Yes                 | Yes        | Yes                   |
| Tuple      | ()          | Yes                 | No         | Yes                   |
| Set        | {}          | No                  | Yes        | No                    |
| Dictionary | {key:value} | Yes                 | Yes        | Keys: No, Values: Yes |

---

# List

A list is used when we need to store multiple values and modify them later.

Example:

```python
fruits = ["Apple", "Banana", "Orange"]
```

Accessing values:

```python
print(fruits[0])
```

Output:

```text
Apple
```

Updating values:

```python
fruits[1] = "Grapes"
```

Result:

```python
["Apple", "Grapes", "Orange"]
```

### Common Uses

* Student names
* Product names
* Marks list
* Shopping items

---

# Tuple

A tuple is similar to a list, but its values cannot be changed once created.

Example:

```python
months = ("Jan", "Feb", "Mar")
```

Accessing values:

```python
print(months[1])
```

Output:

```text
Feb
```

Trying to update:

```python
months[0] = "April"
```

Produces an error.

### Common Uses

* Months
* Days of week
* Coordinates
* Fixed settings

---

# Set

A set stores only unique values.

Example:

```python
numbers = {1, 2, 3, 2, 1}
```

Output:

```python
{1, 2, 3}
```

Duplicate values are removed automatically.

Adding a value:

```python
numbers.add(4)
```

### Common Uses

* Removing duplicates
* Unique departments
* Unique usernames
* Membership checking

Example:

```python
if "IT" in departments:
    print("Found")
```

---

# Dictionary

A dictionary stores data in key-value format.

Example:

```python
student = {
    "name": "Maha",
    "mark": 90
}
```

Accessing values:

```python
print(student["name"])
```

Output:

```text
Maha
```

Adding a new item:

```python
student["dept"] = "Data Science"
```

Result:

```python
{
    "name": "Maha",
    "mark": 90,
    "dept": "Data Science"
}
```

### Common Uses

* Student records
* Employee details
* Product information
* Login data

---

# Real-Life Examples

## List

```python
students = ["John", "Ram", "Maha"]
```

Just a collection of names.

---

## Tuple

```python
months = ("Jan", "Feb", "Mar")
```

Fixed values that rarely change.

---

## Set

```python
departments = {"IT", "Finance", "IT", "HR"}
```

Output:

```python
{"IT", "Finance", "HR"}
```

Duplicate values are removed.

---

## Dictionary

```python
student = {
    "name": "Maha",
    "dept": "Data Science",
    "mark": 90
}
```

Every value has a label.

---

# Easy Way to Remember

### List

Collection of items that can be updated.

### Tuple

Collection of items that stay fixed.

### Set

Collection of unique items.

### Dictionary

Collection of key-value pairs.

---

# One-Line Answer

List is ordered and mutable. Tuple is ordered and immutable. Set stores unique unordered values. Dictionary stores data as key-value pairs and allows values to be accessed using keys.
