[slide]
# Reading User Input
Everything we receive from the console comes as a string

Reading user input is done with a simple command:
```python
name = input()
```
Everything we print on the console is converted to string
```python
print("Hello World!")
```
[/slide]

[slide]
# Formatting Output
Formatting text with **placeholders**:
```python
first_name = "John"
last_name = "Doe"
print(f"{first_name} {last_name}") # John Doe
```
Formatting numbers with **placeholders**:
```python
a = 5.123
print(f"{a:.2f}") # 5.12
```
[/slide]

[slide]
# Reading User Input
A program which **reads** a name from the console and **prints** it:
```python
name = input()
print(name)
```
The result from the execution would be:
```python
Input: John
Output: John
```
[/slide]

[slide]
# Reading Integers
Reading an integer number:
```python
num = int(input())
```
Example:

* Calculating square's area by given side a:
```python
a = int(input())
area = a * a
print(area)
```
[/slide]

[slide]
# Reading Floating-point Numbers
Reading a floating-point number:
```python
num = float(input())
```
Example:

* Convert **inches** to **centimeters**
```python
inches = float(input())
centimeters = inches * 2.54
print(centimeters)
```
[/slide]

[slide]
# Importing Libraries (import)
Sometimes we need to import external libraries
```python
import name of the library
```
Examples
```python
import math      # import math library
import sys       # import sys library
import math, sys # import both math and sys libraries
```
[/slide]

[slide]
# Executing Python
Open the terminal in your working folder and execute
```
python {file_name}
```
[image src="https://github.com/AlenPaunov/pb-interactive-course/blob/01-python-expressions-and-statements/assets/expressions-and-statements-1.png"/]
[/slide]

[slide]
# Problem: Greeting
[code-task title="Greeting" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a user input - name, from the console
* Prints "Hello, \{name\}", where \{name\} is the user input
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|John|Hello, John|
|Dave|Hello, Dave|
[/slide]

[slide]
# Solution: Greeting
[code-task title="Greeting" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
name = input()
print('Hello, ', end="")
print(name)
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a user input - name, from the console
* Prints "Hello, \{name\}", where \{name\} is the user input
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|John|Hello, John|
|Dave|Hello, Dave|
[/slide]
