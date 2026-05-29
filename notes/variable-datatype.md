# Variable
In python, variable is a name that refers to a value stored in memory.
```bash
user_name = "john doe"
age = 21
isActive = True
x, y, z = 1, 2, 3   # multiple variable assignment in single line
x = y = z = 1       # same value assigned to multiple variables
```
## Variable naming convention
A variable can have a short name (like x and y) or a more descriptive name (age, carname, total_volume).
- Allowed: username, user_name, user1, _username, userName(allowed but camelCase not recommended in python)
- Not Allowed: 1user, user-name, class (or any language specific keyword)
- In python, snake_case pattern is followed in industry.
## Python is dynamically typed language
Means, you do not declare the type explicitly, python automatically determines type, and can even change type after they have been set.
```bash
x = 10          # x is of type int
x = "hello"     # now x is of type str
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
### Example
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
## Datatypes
Type of data stored in a variable.
## Types - 
### Numeric Type
```bash
a = 10         # int
b = -10        # int
c = 10.5       # float
```
### String
```bash
name = "john doe"
print(name[0]) # j 
name[0] = "f"  # String is immutable, so changing it is not possible once created
```
#### String Operations 
**Concatinaion -**
```bash
text1 = "hello"
text2 = "world"
print(text1 + " " + text2)   # hello world
```
**Repitition -**
```bash
print("hi" * 3)              # hihihi
```
### Boolean
Boolean represents one of two values: True or False
```bash
isActive = True
if (isActive):
    print("User is active")
else:
    print("User not active")
```
### List
Lists are used to store multiple items in a single variable. List items are ordered, indexed, mutable, and duplication is allowed.
```bash
num_list = [10,20,30]
cloud_providers_list = ["aws","azure","gcp"]
mixed_data_list = [10, "hello", True]         # List with different types of data
print(num_list[0])                            # 10
print(type(num_list))                         # List
```
### Tuples
Tuples are also used to store multiple items in a single variable. Tuple items are ordered, indexed, immutable, and duplication is allowed.
```bash
num_tuple = (10,20,30)
cloud_providers_tuple = ("aws","azure","gcp")
mixed_data_tuple = [10, "hello", True]         # Tuple with different types of data
print(num_Tuple[0])                            # 10
print(type(num_tuple))                         # tuple
```
### Sets
Like list and tuple, sets are also used to store multiple items in a single variable. Set items are unordered, unindexed, immutable, and duplication is not allowed.
```bash
num_set = {10,20,30,30}
cloud_providers_set = {"aws","azure","gcp"}
mixed_data_set = [10, "hello", True]            # Set with different types of data
print(num_set)                                  # {10,20,30}
print(type(num_set))                            # set
num_set[0] = 100                                # error - not allowed
```
> True and 1, False and 0 are considered as the same value in sets, are treated as duplicates
### Dictionaries
Dictionaries are used to store data values in key:value pairs. Dictionary items are ordered, mutable, and duplication is not allowed.
```bash
instance_obj = {
    "name": "ai-bankapp-server",
    "type": "t2.micro",
    "cpu": 2,
    "isUp": False
    "volume": {
         "volume_size": 8,
         "volume_type": "gp3"
    }
}
instance_obj["cpu"] = 3                           # update dictionary
print(instance_obj["volume"])                     # {'volume_size': 8, 'volume_type': 'gp3'}
print(type(instance_obj))                         # dict
```
### None
The None keyword is used to define a null value, or no value at all. It is not the same as 0, False, or an empty string.
```bash
x = None
```
## Mutable vs Immutable
| Mutable | Immutable |
| --------------- | --------------- |
| can change, add/remove data after creation   | cannot change, add/remove data after creation   |
| List, Dictionary   | Numeric, String, Boolean, Tuple, Set, none   |
## Type checking and Type conversion (Casting)
type() is a built-in function, used to find the type of value passed inside it.
```bash
x = 10
print(type(x))                                       # int
print(type([1,2,3])                                  # list
```
Type conversion(casting) is the process of converting a variable or a value from one type to another.
```bash
x = 10
print(str(x))                                        # "10"          
print(int(10.5))                                     # 10
print(bool(1))                                       # True
print(bool(""))                                      # False
print(int("hello"))                                  # Error
```
