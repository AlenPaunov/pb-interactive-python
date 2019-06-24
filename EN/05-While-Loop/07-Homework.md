[slide]
# Homework
Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem.
[/slide]

[slide]
# Problem: Sum Digits
[code-task title="Sum Digits" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a number from the console
* Sums the digits of a number
* Prints the sum
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5634|18|
[/slide]

[slide]
# Solution: Sum Digits
[code-task title="Sum Digits" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
n = int(input())
sum = 0
while n > 0:
   sum += n % 10
   n = int(n / 10);
print(sum);
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a number from the console
* Sums the digits of a number
* Prints the sum
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5634|18|
[/slide]

[slide]
# Problem: Favorite Book
[code-task title="Favorite Book" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which: 

* Reads a book's name from the console
* Receives names until it gets the same book
* Prints "Book found!" and stops afterwards
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|Alice in Wonderland|Book Found!|
|Winnie the Pooh||
|Peter Pan||
|Alice in Wonderland||
[/slide]

[slide]
# Solution: Favorite Book
[code-task title="Favorite Book" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
favorite_book = input()
book = input()
while book != favorite_book:
  book = input()
print("Book found!")
```
[/code-editor]
[task-description]
Write a program, which: 

* Reads a book's name from the console
* Receives names until it gets the same book
* Prints "Book found!" and stops afterwards
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|Alice in Wonderland|Book Found!|
|Winnie the Pooh||
|Peter Pan||
|Alice in Wonderland||
[/slide]

[slide]
# Problem: Find Min and Max
[code-task title="Find Min and Max" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
import math

# Write your code here
```
[/code-editor]
[task-description]
Write a program, which: 

* Receives integers until "END"
* Prints the biggest and the smallest integer
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|Max number: 304|
|20|Min number: 0|
|304||
|0||
|50||
|END||
[/slide]

[slide]
# Solution: Find Min and Max
[code-task title="Find Min and Max" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
import math

line = input()
min = math.inf
max = -math.inf
while line != "END":
  n = int(line)
  if n < min:
    min = n
  if n > max:
    max = n
  line = input() 
print(f"Max number: {max}")
print(f"Min number: {min}")
```
[/code-editor]
[task-description]
Write a program, which: 

* Receives integers until "END"
* Prints the biggest and the smallest integer
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|Max number: 304|
|20|Min number: 0|
|304||
|0||
|50||
|END||
[/slide]

[slide]
# Problem: Special Number
[code-task title="Special Number" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which: 

* Receives integer
* Prints "\{num\} is special" if the number is special
    * Special number is number divisible by all of its digits without remainder
* Otherwise, prints "\{num\} is not special"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|23|23 is not special|
|44|44 is special|
[/slide]

[slide]
# Solution: Special Number
[code-task title="Special Number" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
origin_number = int(input())
number = origin_number
is_special = True
while number > 0:
  digit = number % 10
  number = int(number / 10)
  if origin_number % digit != 0:
    is_special = False
    break
if is_special:
  print(f"{origin_number} is special")
else:
  print(f"{origin_number} is not special")
```
[/code-editor]
[task-description]
Write a program, which: 

* Receives integer
* Prints "\{num\} is special" if the number is special
    * Special number is number divisible by all of its digits without remainder
* Otherwise, prints "\{num\} is not special"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|23|23 is not special|
|44|44 is special|
[/slide]

[slide]
# Problem: Special Bonus
[code-task title="Special Bonus" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a special integer number from the console
* Keeps reading integers until it finds the same one
* When it finds it, it increases the value of the previous number before it with 20% and prints it
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|25|36.0|
|20||
|30||
|25||
[/slide]

[slide]
# Solution: Special Bonus
[code-task title="Special Bonus" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
special = int(input())
number = int(input())
previous = number
while True:
  if number == special:
    previous += previous * 0.2
    break
  previous = number
  number = int(input())
print(previous)
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a special integer number from the console
* Keeps reading integers until it finds the same one
* When it finds it, it increases the value of the previous number before it with 20% and prints it
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|25|36.0|
|20||
|30||
|25||
[/slide]

[slide]
# Problem: Sequence 2k + 1
[code-task title="Sequence 2k + 1" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which: 

* Reads a number n from the console
* Prints a sequence of numbers, which are <= n and satisfy the following condition:
    * Each number is equal to the previous onemultiplied by 2 plus 1
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|8|1|
||3|
||7|
|||
[/slide]

[slide]
# Solution: Sequence 2k + 1
[code-task title="Sequence 2k + 1" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
n = int(input())
k = 1
while k <= n:
  print(k)
  k = k * 2 + 1
```
[/code-editor]
[task-description]
Write a program, which: 

* Reads a number n from the console
* Prints a sequence of numbers, which are <= n and satisfy the following condition:
    * Each number is equal to the previous one multiplied by 2 plus 1
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|8|1|
||3|
||7|
|||
[/slide]

[slide]
# Problem: Account Balance
[code-task title="Account Balance" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which: 

* Receives an integer n - count of transactions
* Receives the amount of money for each transaction
* Adds the money to the balance and prints: "Increase: \{money\}" and calculates and prints the total balance
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|Increase: 5.51|
|5.51|Increase: 69.42|
|69.42|Increase: 100.00|
|100|Total: 174.93|
[/slide]

[slide]
# Solution: Account Balance
[code-task title="Account Balance" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
n = int(input())
balance = 0.0
while n != 0:
  amount = float(input())
  balance += amount
  print(f"Increase: {amount:.2f}")
  n -= 1
print(f"Total: {balance:.2f}")
```
[/code-editor]
[task-description]
Write a program, which: 

* Receives an integer n - count of transactions
* Receives the amount of money for each transaction
* Adds the money to the balance and prints: "Increase: \{money\}" and calculates and prints the total balance
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|Increase: 5.51|
|5.51|Increase: 69.42|
|69.42|Increase: 100.00|
|100|Total: 174.93|
[/slide]

[slide]
# Problem: Reverse Numbers
[code-task title="Reverse Numbers" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
Write a program, which:

* Receives a five-digit number: integer
* Prints that number reversed: integer

Use while loop

You are not allowed to use strings
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|12345|54321|
[/slide]

[slide]
# Solution: Reverse Numbers
[code-task title="Reverse Numbers" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
num = int(input())
result = 0
counter = 10000
while num != 0:
    result += int((num % 10)) * counter
    counter /= 10
    num /= 10
print(int(result))
```
[/code-editor]
[task-description]
Write a program, which:

* Receives a five-digit number: integer
* Prints that number reversed: integer

Use while loop

You are not allowed to use strings
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|12345|54321|
[/slide]