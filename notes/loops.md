# Loops
Loops are used to execute a block of code repeatedly based on specific condition. Python uses two primary types of loops to 
handle repititive tasks: for loops and while loops.
## For Loop
A for loop is used to iterate over a sequence (like a list, tuple, dictionary or a string). It executes a block of code once
for each item in that sequence.
### Example - 1
```bash
for i in range(10):
  print(i)
```
### Example - 2
```bash
num_list = [10,20,30,40,50]
for num in num_list:
  print(num)
```
## While Loop
While loop repeaedly executes a block of code as long as a given condition remains true. It is typically used when you don't 
know exactly how many times the loop should run.
### Example - 3
```bash
count = 0
while count<3:
  print(count)
  count+=1   # crucial to avoid infinite loop
```
