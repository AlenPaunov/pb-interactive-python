[slide]
# Homework

Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem.
[/slide]

[slide]
# Problem: Number Sequence
[code-task title="Number Sequence" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n representing the count of numbers to read next
* Finds the max and the min numbers
* Prints them on the console
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|Max number: 304|
|10|Min number: 0|
|20||
|304||
|0||
|50||
[/slide]

[slide]
# Solution: Number Sequence
[code-task title="Number Sequence" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
n = int(input())
min = n
max = n
for i in range(0,n):
    num = int(input())
    if num < min:
        min = num
    if num > max:
        max = num
print(f"Max number: {max}")
print(f"Min number: {min}")
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n representing the count of numbers to read next
* Finds the max and the min numbers
* Prints them on the console
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|Max number: 304|
|10|Min number: 0|
|20||
|304||
|0||
|50||
[/slide]

[slide]
# Problem: Power of Number
[code-task title="Power of Number" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Reads p - the power and n - the number
* Prints the result of n powered by p
* Don't use math.pow()
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|32|
|2||

|Input|Output|
|-----|------|
|4|81|
|3||
[/slide]

[slide]
# Solution: Power of Number
[code-task title="Power of Number" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
p = int(input())
n = int(input())
result = 1
for i in range(0, p):
  result = result * n
print(result)
```
[/code-editor]
[task-description]
Write a program, which:

* Reads p - the power and n - the number
* Prints the result of n powered by p
* Don't use math.pow()
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|32|
|2||

|Input|Output|
|-----|------|
|4|81|
|3||
[/slide]

[slide]
# Problem: Equal Pairs
[code-task title="Equal Pairs" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Reads number n and n pairs of numbers
* Prints "Yes, value={sum}", if the sum of all pairs is the same
* Otherwise, prints "No, maxdiff={diff}"
    * diff is the max difference in the sum between two pairs
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|Yes, value=-1|
|-1||
|0||
|0||
|-1||
[/slide]

[slide]
# Solution: Equal Pairs
[code-task title="Equal Pairs" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
n = int(input())
prev_sum = 0
max_diff = 0
are_equal = True
for i in range(0, n):
  a = int(input())
  b = int(input())
  if i > 0:
    if max_diff < abs(prev_sum - a - b):
      max_diff = abs(prev_sum - a - b)
    if are_equal and a + b != prev_sum: 
      are_equal = False
  prev_sum = a + b
if are_equal:
  print(f"Yes, value={prev_sum}")
else:
  print(f"No, maxdiff={max_diff}")
```
[/code-editor]
[task-description]
Write a program, which:

* Reads number n and n pairs of numbers
* Prints "Yes, value={sum}", if the sum of all pairs is the same
* Otherwise, prints "No, maxdiff={diff}"
    * diff is the max difference in the sum between two pairs
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|Yes, value=-1|
|-1||
|0||
|0||
|-1||
[/slide]

[slide]
# Problem: Biggest Number
[code-task title="Biggest Number" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n - number representing amount of input numbers
* Reads n numbers
* Finds and prints the biggest number
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|90|
|40||
|90||
|50||

|Input|Output|
|-----|------|
|3|-40|
|-40||
|-90||
|-50||
[/slide]

[slide]
# Solution: Biggest Number
[code-task title="Biggest Number" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
n = int(input())
first_num = int(input())
max_number = first_num
for i in range(1, n):
  number = int(input())
  if number > max_number:
    max_number = number
print(max_number)
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n - number representing amount of input numbers
* Reads n numbers
* Finds and prints the biggest number
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|90|
|40||
|90||
|50||

|Input|Output|
|-----|------|
|3|-40|
|-40||
|-90||
|-50||
[/slide]

[slide]
# Problem: Zig Zag Sum
[code-task title="Zig Zag Sum" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n - number representing amount of input numbers
* Reads n numbers 
        * For every even line adds the number to the result
* For every odd line subtracts the number from the result
* Prints the result
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|-30|
|10||
|-20||
[/slide]

[slide]
# Solution: Zig Zag Sum
[code-task title="Zig Zag Sum" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
n = int(input())
sum = 0
for i in range(1, n+1):
  m = int(input())
  if i % 2 == 0:
    sum += m
  else:
    sum -= m
print(sum)
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n - number representing amount of input numbers
* Reads n numbers 
        * For every even line adds the number to the result
* For every odd line subtracts the number from the result
* Prints the result
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|-30|
|10||
|-20||
[/slide]

[slide]
# Problem: Divide Without Remainder
[code-task title="Divide Without Remainder" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n and n numbers
* Finds in percentage how many of them can divide without remainder at 2, 3 and 4
* Prints percentages p1, p2 and p3, formatted to the second digit
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|33.33%|
|3|100.00%|
|6|0.00%|
|9||

|Input|Output|
|-----|------|
|3|66.67%|
|4|66.67%|
|6|33.33%|
|3||
[/slide]

[slide]
# Solution: Divide Without Remainder
[code-task title="Divide Without Remainder" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
n = int(input())
p1 = 0.0
p2 = 0.0
p3 = 0.0
for i in range(0, n):
  num = int(input())
  if num % 2 == 0:
     p1+=1
  if num % 3 == 0:
     p2+=1
  if num % 4 == 0:
     p3+=1
result_P1 = (p1 / n) * 100;
result_P2 = (p2 / n) * 100;
result_P3 = (p3 / n) * 100;
print(f"{result_P1:.2f}%")
print(f"{result_P2:.2f}%")
print(f"{result_P3:.2f}%")
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n and n numbers
* Finds in percentage how many of them can divide without remainder at 2, 3 and 4
* Prints percentages p1, p2 and p3, formatted to the second digit
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|33.33%|
|3|100.00%|
|6|0.00%|
|9||

|Input|Output|
|-----|------|
|3|66.67%|
|4|66.67%|
|6|33.33%|
|3||
[/slide]

[slide]
# Problem: Vowel Sum
[code-task title="Vowel Sum" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n - the count of characters:
* If character is vowel adds its value to the result

|character|a|e|i|o|u|
|---------|-|-|-|-|-|
|value|1|2|3|4|5|

* Prints the result
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|1|
|a||
|g||

|Input|Output|
|-----|------|
|2|8|
|i||
|u||
[/slide]

[slide]
# Solution: Vowel Sum
[code-task title="Vowel Sum" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
n = int(input())
vowel_sum = 0
for i in range(0, n):
  letter = input()
  if letter == 'a': 
    vowel_sum += 1
  elif letter == 'e': 
    vowel_sum += 2
  elif letter == 'i':
    vowel_sum += 3
  elif letter == 'o':
    vowel_sum += 4
  elif letter == 'u':
    vowel_sum += 5
print(vowel_sum)
```
[/code-editor]
[task-description]
Write a program, which:

* Reads n - the count of characters:
* If character is vowel adds its value to the result

|character|a|e|i|o|u|
|---------|-|-|-|-|-|
|value|1|2|3|4|5|

* Prints the result
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|1|
|a||
|g||

|Input|Output|
|-----|------|
|2|8|
|i||
|u||
[/slide]

[slide]
# Problem: Rollercoaster
[code-task title="Rollercoaster" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Reads rollercoaster places, minimum age, count of  people on the queue and age for each person
    * If all places are taken, prints - "The rollercoaster departures"
    * In other case, prints "Waiting..."
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|The rollercoaster departures|
|10||
|1||
|15||
[/slide]

[slide]
# Solution: Rollercoaster
[code-task title="Rollercoaster" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
rollercoaster_places = int(input())
min_age = int(input())
people_count = int(input())
valid_people_count = 0
for i in range(0, people_count):
  person_age = int(input())
  if person_age >= min_age and rollercoaster_places > valid_people_count:
      valid_people_count+=1
if valid_people_count == rollercoaster_places:
  print("The rollercoaster departures")
else:
  print("Waiting...")
```
[/code-editor]
[task-description]
Write a program, which:

* Reads rollercoaster places, minimum age, count of  people on the queue and age for each person
    * If all places are taken, prints - "The rollercoaster departures"
    * In other case, prints "Waiting..."
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|The rollercoaster departures|
|10||
|1||
|15||
[/slide]

[slide]
# Problem: Multiply
[code-task title="Multiply" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which: 

* Reads n 
* Prints n's multiples in the format "\{n\} x \{i\} = \{result\}"
  * Where i are the numbers from 1 to 10 (inclusive)
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|2 x 1 = 2|
||2 x 2 = 4|
||2 x 3 = 6|
||2 x 4 = 8|
||2 x 5 = 10|
||2 x 6 = 12|
||2 x 7 = 14|
||2 x 8 = 16|
||2 x 9 = 18|
||2 x 10 = 20|
[/slide]

[slide]
# Solution: Multiply
[code-task title="Multiply" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
n = int(input())
for i in range(1, 11):
  result = n * i
  print(f"{n} x {i} = {result}")
```
[/code-editor]
[task-description]
Write a program, which: 

* Reads n 
* Prints n's multiples in the format "\{n\} x \{i\} = \{result\}"
  * Where i are the numbers from 1 to 10 (inclusive)
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|2 x 1 = 2|
||2 x 2 = 4|
||2 x 3 = 6|
||2 x 4 = 8|
||2 x 5 = 10|
||2 x 6 = 12|
||2 x 7 = 14|
||2 x 8 = 16|
||2 x 9 = 18|
||2 x 10 = 20|
[/slide]