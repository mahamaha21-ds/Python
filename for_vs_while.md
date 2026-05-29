# **FOR VS WHILE LOOP TASKS**

## **Task 1: Print Numbers**

```python
for i in range(1, 11):
    print(i)
```

## **Task 2: Even Numbers**

```python
for i in range(1, 21):
    if i % 2 == 0:
        print(i)
```

## **Task 3: Sum of Numbers**

```python
total = 0
for i in range(1, 11):
    total = total + i
print(total)
```

## **Task 4: Multiplication Table**

```python
number = int(input("Enter a number of the table:"))
for i in range(1, 11):
    print(i, "*", number, "=", i * number)
```

## **Task 5: List Iteration**

```python
nums = [10, 20, 30, 40]
for i in nums:
    print(i)
```

# **WHILE LOOP TASKS**

## **Task 6: Print 1 to 10**

```python
i = 1
while i <= 10:
    print(i)
    i += 1
```

## **Task 7: Countdown**

```python
i = 10
while i >= 1:
    print(i)
    i = i - 1
```

## **Task 8: Sum Until User Stops**

```python
total = 0
while True:
    number = int(input("enter a number:"))
    if number == 0:
        print("Stop")
        break
    total = total + number
print(total)
```

## **Task 9: Password Retry**

```python
keyword = "maha"
password = input("Enter a password:")
while True:
    if password == keyword:
        print("correct password")
        break
    else:
        password = input("Enter a correct password:")
```

# **COMBINED (FOR + WHILE + IF)**

## **Task 10: Even Numbers in List**

```python
num = [1, 2, 3, 4, 5, 6]
for i in num:
    if i % 2 == 0:
        print(i)
```

## **Task 11: Number Guessing Game**

```python
num = 7
guess = int(input("Guess the number:"))
while True:
    if guess == num:
        print("You Guessed Correct:", guess)
        break
    else:
        guess = int(input("Guess the number:"))
```

# **REAL-TIME TASKS**

## **Task 12: ATM Simulation**

```python
user = int(input("Enter an amount:"))
balance = 1000
while True:
    if user <= balance:
        withdraw = balance - user
        print("balance:", withdraw)
        print("EXIT")
        break
    else:
        last = input("Insufficient amount(EXIT? Enter 'exit'):").lower()
        if last == "exit":
            print("EXIT")
            break
```

## **Task 13: Shopping Cart Loop**

```python
items = ['banana', 'apple', 'grapes', 'orange', 'dragonfruit']
price = [50, 100, 150, 100, 90]
for i in range(len(items)):
    print(items[i], "-", price[i])

user = input("Enter item name:")
if user in items:
    idx = items.index(user)
    print(items[idx], "costs", price[idx])
```

## **Task 14: Prime Number Check**

```python
primenum = (2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47)
user = int(input("Enter a number:"))
if user in primenum:
    print("It is PrimeNumber")
else:
    print("It's not a PrimeNumber")
```
