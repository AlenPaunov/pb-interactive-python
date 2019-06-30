[slide]
# Homework
Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem.
[/slide]

[slide]
# Problem: Building
[code-task title="Building" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Prints information about apartments (odd rows), offices (even rows) and the last floor (last row)
* Apartment "A\{buildingNum\}\{apartmentNum\}"
* Office "O\{floorNum\}\{officeNum\}"
* Floor "L\{buildingNum\}\{apartmentNum\}"
* The numbers always start from 0
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|6|L60 L61 L62 L63 |
|4|A50 A51 A52 A53 |
||O40 O41 O42 O43 |
||A30 A31 A32 A33 |
||O20 O21 O22 O23 |
||A10 A11 A12 A13 |
[/slide]

[slide]
# Solution: Building
[code-task title="Building" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
floors = int(input())
rooms = int(input()) 
for i in range(floors, 0, -1):
  for j in range(0, rooms):
    if i == floors:
      print(f"L{i}{j}", end=" ") 
    elif i % 2 == 0:
      print(f"O{i}{j}", end=" ")
    elif i % 2 == 1:
      print(f"A{i}{j}", end=" ")
  print()
```
[/code-editor]
[task-description]
Write a program, which:

* Prints information about apartments (odd rows), offices (even rows) and the last floor (last row)
* Apartment "A\{buildingNum\}\{apartmentNum\}"
* Office "O\{floorNum\}\{officeNum\}"
* Floor "L\{buildingNum\}\{apartmentNum\}"
* The numbers always start from 0
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|6|L60 L61 L62 L63 |
|4|A50 A51 A52 A53 |
||O40 O41 O42 O43 |
||A30 A31 A32 A33 |
||O20 O21 O22 O23 |
||A10 A11 A12 A13 |
[/slide]

[slide]
# Problem: Passwords
[code-task title="Passwords" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Generates custom 3 digit passwords, which meet the following conditions:
* The first digit is an even number
* The second digit is an odd number
* The third is the product of the first two
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|6|212 236 2510 414 4312 4520 616 6318 6530 |
|5|212 236 2510 414 4312 4520 |
[/slide]

[slide]
# Solution: Passwords
[code-task title="Passwords" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
n = int(input())
for i in range(1, n + 1):
  for j in range(1, n + 1):
    if i % 2 == 0 and j % 2 != 0:
      print(f"{i}{j}{i * j} ", end=" ")
```
[/code-editor]
[task-description]
Write a program, which:

* Generates custom 3 digit passwords, which meet the following conditions:
* The first digit is an even number
* The second digit is an odd number
* The third is the product of the first two
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|6|212 236 2510 414 4312 4520 616 6318 6530 |
|5|212 236 2510 414 4312 4520 |
[/slide]

[slide]
# Problem: Magic Number
[code-task title="Magic Number" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Read a number - n, from the console

Find all 3-digit numbers, which:

* Form n as the product of the multiplication of their digits
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|113|
||131|
||311|

|Input|Output|
|-----|------|
|1|111|
[/slide]

[slide]
# Solution: Magic Number
[code-task title="Magic Number" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
magic_number = int(input())
for i in range(1, 10):
  for j in range(1, 10):
    for k in range(1, 10):
      if i * j * k == magic_number:
        print(f"{i}{j}{k}")
```
[/code-editor]
[task-description]
Read a number - n, from the console

Find all 3-digit numbers, which:

* Form n as the product of the multiplication of their digits
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|113|
||131|
||311|

|Input|Output|
|-----|------|
|1|111|
[/slide]

[slide]
# Problem: Travelling
[code-task title="Travelling" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a destination and needed budget for destination
* You must continue reading amount of money until you have enough for the destination
* If you receive the command "End" end the program
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|Greece|Going to Greece!|
|1000||
|550||
|450||
|End||
[/slide]

[slide]
# Solution: Travelling
[code-task title="Travelling" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
town_name = input()
current_money = 0
needed_money = float(input())
new_money = float(input())
while new_money != "End":
  new_money = float(new_money)
  current_money += new_money
  if current_money >= needed_money:
    print(f"Going to {town_name}")
    break
  new_money = input()
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a destination and needed budget for destination
* You must continue reading amount of money until you have enough for the destination
* If you receive the command "End" end the program
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|Greece|Going to Greece!|
|1000||
|550||
|450||
|End||
[/slide]

[slide]
# Problem: Prime Numbers
[code-task title="Prime Numbers" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
import math

# Write your code here
```
[/code-editor]
[task-description]
Read two number from the console

Print the prime number in that range
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|1 2 3 5 7 11 13 17 19 23 29 31 37 41 43 47|
|50||
[/slide]

[slide]
# Solution: Prime Numbers
[code-task title="Prime Numbers" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
import math

n = int(input())
m = int(input())

for num in range(n, m + 1):
  prime = True
  divider = 2
  max_divider = int(math.sqrt(num))
  while divider <= max_divider:
    if num % divider == 0:
      prime = False
      break
    divider += 1
  if prime:
    print(num, end=" ")
```
[/code-editor]
[task-description]
Read two number from the console

Print the prime number in that range
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|1 2 3 5 7 11 13 17 19 23 29 31 37 41 43 47|
|50||
[/slide]

[slide]
# Problem: Unique PIN Codes
[code-task title="Unique PIN Codes" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Reads 3 digits - each of them is an upper limit
* Generates unique  3 digit PIN Codes, which meet the following conditions:
    * They are in the range
    * The first and the third digit must be even
    * The second digit must be a prime number in the range \[2…7\]
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|222|
|5|224|
|5|232|
||234|
||252|
||254|
[/slide]

[slide]
# Solution: Unique PIN Codes
[code-task title="Unique PIN Codes" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
n1 = int(input())
n2 = int(input())
n3 = int(input())
for  first_digit in range(1, n1 + 1):
  for second_digit in range(1, n2 + 1):
    for third_digit in range(1, n3 + 1):
      if first_digit % 2 == 0 and third_digit % 2 == 0 and (third_digit == 2 or third_digit == 3 or third_digit == 5 or third_digit == 7):
        print(f"{first_digit}{second_digit}{third_digit}")
```
[/code-editor]
[task-description]
Write a program, which:

* Reads 3 digits - each of them is an upper limit
* Generates unique  3 digit PIN Codes, which meet the following conditions:
    * They are in the range
    * The first and the third digit must be even
    * The second digit must be a prime number in the range \[2…7\]
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|222|
|5|224|
|5|232|
||234|
||252|
||254|
[/slide]

[slide]
# Problem: Letters Combinations
[code-task title="Letters Combinations" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Prints letters combinations and the count of the printed combinations
* You will receive the range of letters on the first and second line
* On the third line, you will receive a letter, which you must ignore - don't print combinations with it
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|a|aaa|
|c|aab|
|b|aba|
||abb|
||baa|
||bab|
||bba|
||bbb|
||8|
[/slide]

[slide]
# Solution: Letters Combinations
[code-task title="Letters Combinations" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
start_letter = input()
end_letter = input()
avoid_letter = input()
counter = 0
for first in range(ord(start_letter), ord(end_letter) + 1):
  for second in range(ord(start_letter), ord(end_letter) + 1):       
    for third in range(ord(start_letter), ord(end_letter) + 1):      
      if chr(first) != avoid_letter and chr(second) != avoid_letter and chr(third) != avoid_letter:
        print(f"{chr(first)}{chr(second)}{chr(third)}")
        counter += 1
print(counter)
```
[/code-editor]
[task-description]
Write a program, which:

* Prints letters combinations and the count of the printed combinations
* You will receive the range of letters on the first and second line
* On the third line, you will receive a letter, which you must ignore - don't print combinations with it
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|a|aaa|
|c|aab|
|b  |aba|
||abb|
||baa|
||bab|
||bba|
||bbb|
||8|
[/slide]

[slide]
# Problem: Number Pattern
[code-task title="Number Pattern" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Receives a single number: n
* Prints the pattern shown in the example
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|1|
||121|
||12321|

|Input|Output|
|-----|------|
|4|1|
||121|
||12321|
||1234321|
[/slide]

[slide]
# Solution: Number Pattern
[code-task title="Number Pattern" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
rows = int(input())
for i in range(1, rows + 1):
  result = ''
  for ascending in range(1, i + 1):
    result += str(ascending)
  for descending in range(i - 1, 0, -1):
    result += str(descending)
  print(result)
```
[/code-editor]
[task-description]
Write a program, which:

* Receives a single number: n
* Prints the pattern shown in the example
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|1|
||121|
||12321|

|Input|Output|
|-----|------|
|4|1|
||121|
||12321|
||1234321|
[/slide]