# Functions
A function is a reusable block of code designed to perform a specific task. It only runs when it is called, helping to avoid code
repitition and making programs more modular.
## Example - 1
```bash
# Function Definition
def sum_of_two_numbers(num1,num2):
  sum = num1 + num2
  return sum
# Function Invocation
sum_result = sum_of_two_numbers(10,20)
print(sum_result)   # 30
```
## Example - 2
```bash
user_name = input("Enter your username: )
def greet_user(user_name="user"):   # default parameter, if argument is passed, overrides it
  print(f"Hello {user_name}")
greet_user(user_name)
```
## Key Components
### Arguments and Parameters
You can pass data into a function as arguments. These values are received by parameters defined in the function's parentheses.
### Return values
Use the return statement to send back data to the caller.
### Default Parameter
You can assign default values to parameters, which are used if no argument is provided during call
