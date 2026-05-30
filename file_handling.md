# **FILE HANDLING TASKS**

## **Task 1: Create & Write File**

```python
import os
path = os.path.join(os.path.expanduser("~"), "Desktop", "notes.txt")

f = open(path, "x")
f.close()

f = open(path, "w")
f.write("Hello Python")
f.close()
```

## **Task 2: Read File**

```python
import os
path = os.path.join(os.path.expanduser("~"), "Desktop", "notes.txt")

f = open(path, "r")
print(f.read())
f.close()
```

## **Task 3: Append Data**

```python
import os
path = os.path.join(os.path.expanduser("~"), "Desktop", "notes.txt")

f = open(path, "a")
f.write("Learning File Handling")
f.close()
```

## **Task 4: Count Characters**

```python
import os
path = os.path.join(os.path.expanduser("~"), "Desktop", "notes.txt")

f = open(path, "r")
content = f.read()
count = len(content)
print(count)
f.close()
```

# **INTERMEDIATE TASKS**

## **Task 5: Count Words**

```python
import os
path = os.path.join(os.path.expanduser("~"), "Desktop", "notes.txt")

f = open(path, "r")
content = f.read()
count = len(content.split())
print(count)
f.close()
```

## **Task 6: Count Lines**

```python
import os
path = os.path.join(os.path.expanduser("~"), "Desktop", "notes.txt")

f = open(path, "r")
lines = f.readlines()
print(len(lines))
f.close()
```

## **Task 7: Store User Input**

```python
f = open("users.txt", "w")
f.write(input("enter the name:"))
f.close()
```

## **Task 8: Multiple User Entries**

```python
f = open("users.txt", "w")
while True:
    name = input("Enter the name:")
    if name == "exit":
        print("exit")
        break
    else:
        f.write(name + "\n")
f.close()
```

# **REAL-TIME TASKS**

## **Task 9: Mini Notes App**

```python
f = open("notes.txt", "w")
f.write("homework\n")
f.write("cleaning\n")
f.write("planting\n")
f.write("gym\n")
f.write("dailynotes\n")
f.close()

f = open("notes.txt", "r")
print(f.read())
f.close()
```

## **Task 10: Student Marks Storage**

```python
import csv
fields = ["name", "mark"]
rows = [["maha", "34"],
        ["raheem", "30"]]
with open("students.csv", "w") as csvfile:
    csvwriter = csv.writer(csvfile)
    csvwriter.writerow(fields)
    csvwriter.writerows(rows)
```

## **Task 11: Login Register System**

```python
username = input()
password = input()
f = open("users.txt", "a")
f.write(username + "\n")
f.write(password + "\n")
f.close()
if username == "maha" and password == "mahe":
    print("successfully login")
else:
    print("Wrong Username or Password")
```

# **JSON FILE TASKS**

## **Task 12: Store Dictionary in JSON**

```python
import json
info = {"name": "maha",
        "age": 22
        }

f = open("data.json", "w")
json.dump(info, f, indent=2)
print(info)
f.close()
```

## **Task 13: Read JSON File**

**Method 1**
```python
import json
f = open("data.json", "r")
data = json.load(f)
print(data.values())
f.close()
```

**Method 2**
```python
import json
info = {
    "stud1": {
            "name": "maha",
            "age": 20
            },
    "stud2": {
            "name": "mahe",
            "age": 21
            },
    }
f = open("data.json", "w")
json.dump(info, f, indent=2)
f.close()

f = open("data.json", "r")
data = json.load(f)
print(data["stud1"]["name"])
print(data["stud2"]["name"])
f.close()
```

# **CHALLENGE TASK**

## **Task 14: Expense Tracker**

```python
item = input("Enter the Item name:")
price = int(input("Enter the price:"))
f = open("expenses.txt", "w")
f.write(item + "-" + str(price) + "\n")
f.close()
print("total:", price)
```
