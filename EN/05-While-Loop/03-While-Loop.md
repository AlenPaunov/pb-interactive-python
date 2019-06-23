[slide]
# While Loop
The **`while`** statement executes a statement or a block of statements while a specified **`boolean expression`** evaluates to **`True`**

The expression is evaluated before each execution of the loop

```python
n = int(input())
# keyword   condition
while n % 2 != 0:
  n = int(input())
print(n)
```
[/slide]

[slide]
# Problem: Decreasing Numbers
[code-task title="Decreasing Numbers" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a number from the console
* Prints the numbers starting from the number to 1 (inclusive)
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|4|4|
||3|
||2|
||1|
[/slide]

[slide]
# Solution: Decreasing Numbers
[code-task title="Decreasing Numbers" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
number = int(input())
while number >= 1:
  print(number)
  number -= 1
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a number from the console
* Prints the numbers starting from the number to 1 (inclusive)
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|4|4|
||3|
||2|
||1|
[/slide]

[slide]
# Problem: Numbers in Range
[code-task title="Numbers in Range" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a number from the console
* Checks if the number is in the range between 1 and 100
    * If it isn't - it reads a new one
    * If it is - prints the number and the program stops
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|-10|50|
|101||
|50||
|||
[/slide]

[slide]
# Solution: Numbers in Range
[code-task title="Numbers in Range" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
num = int(input())
while num < 1 or num > 100:
  num = int(input())
print(num)
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a number from the console
* Checks if the number is in the range between 1 and 100
    * If it isn't - it reads a new one
    * If it is - prints the number and the program stops
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|-10|50|
|101||
|50||
|||
[/slide]