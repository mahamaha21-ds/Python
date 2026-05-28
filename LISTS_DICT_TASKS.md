# **LISTS TASKS**

## **Task 1: Basic List Creation**

```python
fruits = ["apple", "banana", "grapes", "orange", "dragonfruit"]
print(fruits)
print(fruits[0])
print(fruits[4])
```

## **Task 2: Add & Remove Items**

```python
numbers = [10, 20, 30]
numbers.append(40)
numbers.remove(20)
print(numbers)
```

## **Task 3: Sum of List**

```python
num = [10, 20, 30]
print(sum(num))
```

## **Task 4: Student Marks List**

```python
num = [40, 49, 60, 55, 45]
print(sum(num))
avg = sum(num) / 5
print(int(avg))
```

## **Task 5: Basic Dictionary**

```python
info = {
    "name": "mxho",
    "age": 25,
    "course": "ds"
}
print(info.values())
```

## **Task 6: Access & Update**

```python
student = {"name": "John", "age": 20}
print("name:", student["name"])
student["age"] = 22
student["marks"] = 55
print(student)
```

## **Task 7: Product Info (Real-Time)**

```python
dic = {"prodname": "TV",
       "price": 30000,
       "quantity": 2
}
tot_cost = dic["price"] * dic["quantity"]
print(tot_cost)
```

## **Task 8: Simple Login System**

```python
user = {"username": "admin", "password": "1234"}
print("login success for", user["username"])
```

## **Task 9: Multiple Students**

```python
students = [
    {"name": "A", "marks": 80},
    {"name": "B", "marks": 70}
]
print(students[0])
print(students[1])
```

## **Task 10: Shopping Cart**

```python
items = {
    "name": "john",
    "price": 3400,
    "quantity": 2
}
pri = items["price"]
qua = items.get("quantity")
summed = pri * qua
print(summed)
```

## **Task 11: Employee Data**

```python
emp = {"name": "john", "salary": 12000}
emp1 = {"name": "ram", "salary": 13000}
emp2 = {"name": "jeva", "salary": 12000}
print(emp, emp1, emp2)

emps = emp["salary"]
emps1 = emp1.get("salary")
emps2 = emp2["salary"]
em = emps + emps1
print(em + emps2)
```

## **Task 12: Mini Contact Book**

```python
contacts = {
    "John": 9876543210,
    "Alice": 9123456780
}
contacts["jerry"] = 3883044938
print(contacts)
for name in contacts:
    if name == "Alice":
        print("searched")
```
