# Variables & Data Types in Python
In python, variable is a name that refers to a value stored in memory.
```bash
user_name = "john doe"
age = 21
isActive = True
x, y, z = 1, 2, 3  # multiple variable assignment in single line
x = y = z = 1      # same value assigned to multiple variables
```
## Variable naming convention
- Allowed: username, user_name, user1, _username, userName
- Not Allowed: 1user, user-name, class (or any language specific keyword)
- In python, snake_case pattern is followed in industry
## Python is dynamically typed language
Means, you do not declare the type explicitly, python automatically determines type.
```bash
x = 10          # integer
x = "hello"     # now string
```
## Variable Scope
**Local Variable -** Inside function, accessible within the function.
```bash
def test():
    x = 10     # Local variable
print(x)       # error: x is not defined
```
**Global Variable -** Outside function, accessible from anywhere in the file.
```bash
x = 10         # Global Variable
def test():
    print(x)   # 10
test()
```
**Example -**
```bash
x = 10
def test():
    x = 20
    print(x)   # 20
test()
print(x)       # 10
```
## Delete Variable
```bash
x = 10
del x
print(x)       # error: x is not defined
```
