[slide]
# Definition and Syntax
Range is a function in python, which generates a collection of numbers in a given range

```python
range(1, 5) # start and end
```

```python
range(1, 10, 2) # start, end, step (optional)
# 1 3 5 7 9
```
[/slide]

[slide]
# Ranges in Loops
We can use ranges in for-loops
```python
for num in range(1, 5):
  print(num)
# 1
# 2
# 3
# 4
```
```python
for num in range(4, 0, -1):
  print(num)
# 4
# 3
# 2
# 1
```
[/slide]

[slide]
# Problem: Print Sum of N Numbers
[code-task title="Print Sum of N Numbers" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Reads number n from the console
* Sums all numbers from 1 to n
* Prints the sum on the console
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|15|
|6|21|
[/slide]

[slide]
# Solution: Print Sum of N Numbers
[code-task title="Print Sum of N Numbers" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
n = int(input())
sum = 0
for i in range(1, n + 1):
   sum += i
print(sum)
```
[/code-editor]
[task-description]
Write a program, which:

* Reads number n from the console
* Sums all numbers from 1 to n
* Prints the sum on the console
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|15|
|6|21|
[/slide]

[slide]
# Problem: Calculate Monthly Salary
[code-task title="Calculate Monthly Salary" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Reads days in the current month and salary per day
* Calculates the salary for the month
* Prints the result on the console
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|30|300|
|10||

|Input|Output|
|-----|------|
|28|560|
|20||
[/slide]

[slide]
# Solution: Calculate Monthly Salary
[code-task title="Calculate Monthly Salary" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
days = int(input())
salaryPerDay = int(input())
totalSalary = 0
for i in range(1, days + 1):
   totalSalary += salaryPerDay
print(totalSalary)
```
[/code-editor]
[task-description]
Write a program, which:

* Reads days in the current month and salary per day
* Calculates the salary for the month
* Prints the result on the console
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|30|300|
|10||

|Input|Output|
|-----|------|
|28|560|
|20||
[/slide]