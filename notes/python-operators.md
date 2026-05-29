# Python Operators
Operators are used to perform operations on variables and values (operands).
## Types 
- Arithmetic Operators
- Assignment Operators
- Comparison Operators
- Logical Operators
- Membership Operators
### Arithmetic Operators
- Used with numeric values to perform arithmetic operations
- Example: +, -, *, /, %, **, //
```bash
a = 13
b = 5
print(a + b)
print(a -b)
print(a * b)
print(a / b)   # Division, returns float
print(a % b)
print(a ** b)  # Exponentiation
print(a // b)  # Floor Division, returns integer
```
### Assignment Operators
- Used to assign values to variables
- Example: =, +=, -=, *=, /=
```bash
a = 10
a += 5   # a = a + 5
print(a) # 15
```
### Comparison Operators
- Used to compare two values or variables
- It returns True or False based on the comparison
- Example: ==, !=, >, <, >=, <=
```bash
a = 10
b = 5
print(a == b)
print(a != b)
print(a > b)
print(a < b)
print(a >= b)
print(a <= b)
```
### Logical Operators
- Used to combine conditional statements
- Example: and, or, not
```bash
age = int(input("Enter your age: "))
isVoterCardHolder = input("Do you have voter card? (True/False)").lower()
if(age >= 18) and (isVoterCardHolder == "true"):
  print("You are eligible to vote")
else:
  print("You are not eligible to vote")
```
### Membership Operator
- Used to test if a sequence is present in an object
- Example: in, not in
```bash
cloud_service_providers = ["aws","azure","gcp","digital ocean","utho"]
print("digital ocean" in cloud_service_providers)   # True
print("azure" not in cloud_service_providers)       # False
```
## Operator Precedence
Operator precedence describes the order in which the operations are performed.
```bash
print(5 + 4 - 7 + 3)   # 5
print(2 + 3 * 4)       # 14
print((2 + 3) * 4)     # 20
```
