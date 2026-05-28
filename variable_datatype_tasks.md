# Variable & Datatype Tasks

---

## Task 1: Personal Info Storage

```python
name = "mia"
age = 33
height = 160
is_student = True
print(name, age, height, is_student)
```

---

## Task 2: Type Checking

```python
a = 10
b = 3.5
c = "Python"
d = True
print(type(a))
print(type(b))
print(type(c))
print(type(d))
```

---

## Task 3: Simple Type Conversion

```python
num = 10
floating = float(num)
print(floating)

floating = 2.5
integer = int(floating)
print(integer)

integer = 4
string = str(integer)
print(string)
```

---

## Task 4: Student Marks System

```python
stud_name = "ajay"
subj_1 = 55
subj_2 = 49
subj_3 = 53
tot_mark = subj_1 + subj_2 + subj_3
print("The total mark:", tot_mark)
avg_mark = tot_mark / 3
print("The avg mark:", avg_mark)
```

---

## Task 5: Salary Breakdown

```python
basic_salary = 35000
bonus = 5000
tax_per = 5
tot_salary = basic_salary + bonus
print(tot_salary)
salary_after_tax = tot_salary - (tot_salary / 100 * tax_per)
print(int(salary_after_tax))
```

---

## Task 6: Temperature Converter

```python
c = 22.5
F = (c * 9/5) + 32
print(F)
```

---

## Task 7: E-commerce Product Info

```python
prod_name = "TV"
price = 30000
quantity = 2
in_stock = True
tot_cost = price * quantity
print(tot_cost)
```

---

## Task 8: User Login Info

```python
username = "raheem"
password = "rxhm"
login_status = True
print("user", username, "is logged in:", login_status)
```

---

## Task 10: Simple Interest Calculator

```python
pri = 40000
rate = 4
time = 2
SI = pri * rate * time / 100
print(int(SI))
```

---

## Task 11: Mini Profile Generator

```python
name = input()
age = input()
fav_num = input()
print(type(name))
print(type(age))
print(type(fav_num))
conv_age = float(age)
print(conv_age)
conv_num = int(fav_num)
print(conv_num)
```
