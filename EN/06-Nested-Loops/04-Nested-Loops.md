[slide]
# Nested Loops
Statements that consist of several **loops** located **inside each other**

**Nested loops** are used:

* To execute an **action**, which **executes** multiple **actions**

* To make more **complex** calculations and variations
[/slide]

[slide]
# Nested For Loops

```python
for i in range(1, 10):
  # Outer Loop 
  for j in range(1, 10):
  # Inner Loop
     # Statement
```
[/slide]

[slide]
# Problem: Triangle of Stars
[code-task title="Triangle of Stars" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Reads the height of a triangle from the console
* Prints a triangle of stars
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|\*|
||\*\*|
||\*\*\*|
||\*\*\*\*|
||\*\*\*\*\*|
[/slide]

[slide]
# Solution: Triangle of Stars
[code-task title="Triangle of Stars" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
height = int(input())
for i in range(1, height + 1):
    for j in range(1, i + 1):
        print("*", end="");
    print()
```
[/code-editor]
[task-description]
Write a program, which:

* Reads the height of a triangle from the console
* Prints a triangle of stars
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|\*|
||\*\*|
||\*\*\*|
||\*\*\*\*|
||\*\*\*\*\*|
[/slide]

[slide]
# Nested While Loops
```python
while condition:
  # Outer Loop 
  while condition: 
    # Inner Loop
      # Statement
```
[/slide]

[slide]
# Problem: Triangle of Stars 2
[code-task title="Triangle of Stars 2" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Reads the height of a triangle from the console
* Prints a triangle of stars
* Use a while loop
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|\*|
||\*\*|
||\*\*\*|
||\*\*\*\*|
||\*\*\*\*\*|
[/slide]

[slide]
# Problem: Triangle of Stars 2
[code-task title="Triangle of Stars 2" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
height = int(input())
i = 1
  while i <= height:
  j = 0
  while j < i:
    print('*', end="")
    j += 1
  print()
  i += 1
```
[/code-editor]
[task-description]
Write a program, which:

* Reads the height of a triangle from the console
* Prints a triangle of stars
* Use a while loop
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|\*|
||\*\*|
||\*\*\*|
||\*\*\*\*|
||\*\*\*\*\*|
[/slide]
