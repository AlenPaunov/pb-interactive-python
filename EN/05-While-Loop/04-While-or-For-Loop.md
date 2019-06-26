[slide]
# While or For Loop
***While*** and ***for*** loops both **repeat** a block of **code**

Use ***for*** when you know the **number of repetitions**

Use ***while*** when you don't know when you will meet the end condition
[/slide]

[slide]
# Problem: Odd Number
[code-task title="Odd Number" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Reads numbers from the console until it gets an **odd number**
* Prints the **odd** number
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|3|
|4||
|8||
|3||
[/slide]

[slide]
# Solution: Odd Number
[code-task title="Odd Number" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
number = int(input())
while (number % 2) == 0:
    number = int(input())
print(number)
```
[/code-editor]
[task-description]
Write a program, which:

* Reads numbers from the console until it gets an **odd number**
* Prints the **odd** number
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|3|
|4||
|8||
|3||
[/slide]

[slide]
# Problem: Number Manipulator
[code-task title="Number Manipulator" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write code here
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a number from the console
* Reads the following commands:
* **Add** - Аdds 1 to the number
* **Subtract** - Subtracts 1 from the number
* **END** -  Prints the number and stops the program
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|6|
|Add||
|END||
[/slide]

[slide]
# Solution: Number Manipulator
[code-task title="Number Manipulator" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
number = int(input())
command = input()

while command != "END":
    if command == "Add":
        number += 1
    elif command == "Subtract":
        number -= 1
    command = input()

print(number)
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a number from the console
* Reads the following commands:
* **Add** - Аdds 1 to the number
* **Subtract** - Subtracts 1 from the number
* **END** -  Prints the number and stops the program
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|6|
|Add||
|END||
[/slide]
