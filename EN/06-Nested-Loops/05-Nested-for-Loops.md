[slide]
# Nested for Loops
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