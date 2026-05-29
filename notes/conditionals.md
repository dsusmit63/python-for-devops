# Conditionals
## If...Else Statement
### Example - 1
```bash
age = int(input("Enter your age: ))
if age>=18:
    print("You can vote")
else
    print("You can't vote")
```
### Example - 2
```bash
is_logged_in = False
if is_logged_in:
    print("Welcome back!")
else:
    print("Please log in")
```
## If...Elif...Else Statement
### Example - 3
```bash
number = int(input("Enter the number: "))
if number>0:
  print("Positive")
elif number<0:
  print("Negative")
else:
  print("Zero")
```
## Match statement
### Example - 4
```bash
day = int(input("Enter day number: "))
match day:
  case 1:
    print("Monday")
  case 2:
    print("Tuesday")
  case 3:
    print("Wednesday")
  case 4:
    print("Thursday")
  case 5:
    print("Friday")
  case 6:
    print("Saturday")
  case 7:
    print("Sunday")
  case _:
    print("Please enter valid day")
```
