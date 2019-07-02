[slide]
# Problem 06
## Description
It's Friday night and you're wondering which movie to watch. You decide to write a program to choose it for you. Until the command "STOP" you will be receiving titles of your favorite movies. The best movie for you will be the one that has the most points. Points are calculated as the sum of the ASCII character values in the movie title. (There will not be a case where we have two films with an equal number of points)

Keep in mind the following:
- For each lowercase letter in the title, you must subtract from the sum twice the length of the movie title.
- For each uppercase letter in the title, the length of the film's title should be subtracted from the sum.
You can have a maximum of 7 movie titles.

## Input
You receive multiple lines from the console until the command "STOP" or until the limit of 7 movies is reached:
- Movie title – string;

## Output
Print on the console:
- If you have reached the limit of 7 movies you must print: "The limit is reached."
- Print the best movie for you: "The best movie for you is {movie title} with {sum of symbols} ASCII sum."
[code-task title="Problem-06" executionStrategy="python-code" requiresInput]
[code-editor language=python]
```
# Write your code here
```
[/code-editor]
[task-description]
## Input
Matrix

Breaking bad

Legend

STOP

## Output
The best movie for you is Breaking bad with 878 ASCII sum.

## Comments
First we get Matrix, the first letter is M with a value of 77, but it is a capital letter and we subtract from it the length of the title  77- 6  = 71, the second letter is a with a value of 97 and we subtract twice the movie title 97 - 12 = 85. Similarly, we proceed with each subsequent letter and receive an amount of 563.
Upon receiving the STOP command, we print the title with the highest value, which is Breaking bad with sum of 878.
[/task-description]
[code-io /]
[/code-task]
[/slide]