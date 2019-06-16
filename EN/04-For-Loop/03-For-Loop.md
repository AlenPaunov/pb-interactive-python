[slide]

# For Loop: Definition and Syntax

Allows code to be executed repeatedly

Repeating while the condition is met

```python
for i in iterable:
  print(i)
```

[/slide]

[slide]

# Iterable

Iterable means collection that can be iterated over:

- Example for that are strings:

```
"This is some random text"
```

- Using for loops, you can iterate through the text and get each character

# Iterating Strings

```python
for char in "John":
  print(char)
# J
# o
# h
# n
```

[/slide]

[slide]

# Problem: Characters

[code-task title="Characters" executionStrategy="python-code" requiresInput]
[code-editor language=python]

```
# Write your code here
```

[/code-editor]
[task-description]
Write a program, which:

- Receives a single string
- Print each character of that string on a new line

[/task-description]
[code-io /]
[/code-task]

# Sample Input and Output

| Input | Output |
| ----- | ------ |
| Hello | H      |
|       | e      |
|       | l      |
|       | l      |
|       | o      |

[/slide]

[slide]

# Solution: Characters

[code-task title="Characters" executionStrategy="python-code" requiresInput]
[code-editor language=python]

```
text = input()
for char in text:
  print(char)
```

[/code-editor]
[task-description]
Write a program, which:

- Receives a single string
- Print each character of that string on a new line

[/task-description]
[code-io /]
[/code-task]

# Sample Input and Output

| Input | Output |
| ----- | ------ |
| Hello | H      |
|       | e      |
|       | l      |
|       | l      |
|       | o      |

[/slide]
