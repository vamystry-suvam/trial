![logo](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS_4f4ULs1QOS0lLcW1q4PNplieIrON0VFuqA&usqp=CAU)
# Jupyter_lab notebook
### __Suvam Mistry__
#### Aim: Data Scientist
##### _I love Data Science because it will help me to learn and create new models which i can later implement to solve many problems._



In this markdown contains a python program which generates random number within user input range, and prompts user to guess the number.

Table of contents:
* User prompts in Console.
* 1 Importing random module.
* 2 Creating a function in python using the "def" keyword.
* 3 Creating if and elif statements + outputs.
* 4 Final statement and its output if the guess is correct.



After creating the program, executing "guesses()" function in the console prompts the user 2 times for input of minimum and maximum values to specify the value range.
```
guesses()
```
first prompt
```
enter minimum value: 20
```
second prompt
```
enter maximum value: 80
```
NOTE: entering any other value(s) apart from numeric data type will show error


After entering user input prompts, the user has to guess a number between initial and final values and enter that into the console. It looks like this below.
```
guess a number between 1st and 2nd value range :
```
____________________________________________________________

importing random module in python 3 as shown below.
```
import random
```
Below shows creating function using "def" keyword followed by function name(guesses) and specifying arguments in parenthesis. Inputs provided by the user using "input()" function which is then converted from string to numeric data type using "float()" function, by default "input()" function converts user input as string data type.
```
def guesses(i=float(input("enter minimum value: ")),x=float(input("enter maximum value: "))):
    random_number = random.randint(i,x)
    guess = 0
```

"while" loop which repeatedly prompts user to enter numeric guess values in the console as shown below.
```
    while guess != random_number:
        guess = float(input("guess a number between 1st and 2nd value range :"))
```

"if" statement below which determines if the user entered "guess" value is greater than "random_number" value then will print output in console "guess is too high".
```
        if guess > random_number:
            print("guess is too high")
```
output from the "if" statement.
```
guess is too high
```

"elif" else-if statement below which determines if the user entered "guess" value is less than "random_number" value then will print output in console "guess is too low".
```
        elif guess < random_number:
            print("guess is too low")
```
output from "elif" statement.
```
guess is too low
```

At last, if the guess is not too high or too low and it is correct then, this line will execute.
```
    print(f"correct guess {random_number}")
```
output
```
correct guess 45
```
__________________________________________________________________________
[This is program was edited from here.](https://youtu.be/8ext9G7xspg)


| Date          |Time     |Timezone|
|---------------|:-------:|-------:|
| 27th May 2022 | 9:10 PM | IST    |
