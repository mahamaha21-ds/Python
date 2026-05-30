# **BASIC FUNCTION TASKS**

## **Task 1: Simple Function**

```python
def create():
    print("Hello Python")
create()
```

## **Task 2: Function with Parameter**

```python
def funct(name):
    print("Hello", name)
funct("maha")
```

## **Task 3: Add Two Numbers**

```python
def adding(num1, num2):
    added = num1 + num2
    return added
tot = adding(3, 5)
print(tot)
```

## **Task 4: Even or Odd Function**

```python
def oddeven(num):
    if num % 2 == 0:
        return "EVEN"
    else:
        return "ODD"

finding = oddeven(5)
print(finding)
```

## **Task 5: Square of Number**

```python
def square(num):
    value = num * num
    return value
z = square(3)
print("square value of given number:", z)
```

# **INTERMEDIATE TASKS**

## **Task 6: Maximum of Two Numbers**

```python
def maximum(num1, num2):
    if num1 > num2:
        return num1
    elif num2 > num1:
        return num2
    else:
        return "NONE"

z = maximum(3, 5)
print(z)
```

## **Task 7: Factorial using Function**

```python
def factorial(num):
    result = 1
    for i in range(1, num+1):
        result = result * i
    return result
print(factorial(5))
```

## **Task 8: Sum of List**

```python
def function():
    item = [10, 20, 30]
    print(sum(item))
function()
```

# **COMBINED TASKS**

## **Task 9: Calculator Function**

```python
def calculator(num1, num2, operator):
    if operator == "+":
        return num1 + num2
    elif operator == "-":
        return num1 - num2
    elif operator == "*":
        return num1 * num2
    elif operator == "/":
        return num1 / num2
storing = calculator(4, 4, "-")
print(storing)
```

## **Task 10: Prime Check Function**

```python
def primecheck(num):
    if num < 2:
        return "Not Prime"
    for i in range(2, num):
        if num % i == 0:
            return "Not Prime"
    return "Prime"
print(primecheck(7))
```

## **Task 11: Password Validator**

```python
def passwordvalidator(password):
    if len(password) < 6:
        return "Invalid"
    has_num = any(c.isdigit() for c in password)
    if has_num:
        return "valid"
    else:
        return "Invalid"

c = passwordvalidator("maha")
print(c)
```

# **REAL-TIME TASKS**

## **Task 12: Student Result Function**

**METHOD 1**
```python
def result():
    m1 = 40
    m2 = 30
    m3 = 40
    total = m1 + m2 + m3

    if total >= 280:
        return "Distinction"
    elif total >= 140 and total <= 279:
        return "Pass"
    else:
        return "Fail"

print(result())
```

**METHOD 2**
```python
def result():
    m1 = 50
    m2 = 59
    m3 = 59
    if m1 >= 90 and m2 >= 90 and m3 >= 90:
        return "Distinction"
    elif m1 >= 50 and m2 >= 50 and m3 >= 50:
        return "Pass"
    else:
        return "Fail"
print(result())
```

## **Task 13: ATM Function System**

```python
def atm(chkbalance):
    print("checking balance, Enter 1")
    print("Withdraw amount, Enter 2")
    enter = int(input("Enter:"))
    balance = 10000
    if enter == 1:
        print("balance amount:", balance)
    elif enter == 2:
        if chkbalance <= balance:
            print("withdraw")
            balance -= chkbalance
            print(balance)
        else:
            print("Insufficient balance")

atm(1000)
```
