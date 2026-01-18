# Lab2
In this lab, you will create **eight simple Python scripts**. All scripts must be written in **GitHub Codespaces**.
This lab focuses on practicing **decision-making** and **iteration** in Python, including:  
- `if` statements  
- `for` loops  
- `while` loops

# Lab Objectives
- Develop understanding in handling user input and validating data
- Apply control flow structures to solve real-world problems
- Master loop constructs for both counter-driven and event-driven tasks
- Implement loop control mechanisms using break and continue
- Document and present code execution results through screenshots and organized submission.
 
# Submission Instructions
For each task:
1. **Write the script** in Codespaces.  
2. **Run the script** from the **terminal**.  
3. **Take a screenshot** that clearly shows:  
   - Your **code** in the editor.  
   - The **terminal output**, including your **username** visible in the terminal.  
4. **Insert the screenshot** into a Word document under the heading that matches the task name:  
   - Example: **Task1**, **Task2**, **Task3**, etc.  
5. After completing all tasks, **convert the Word document to PDF**.  Name the PDF file using your **Seneca username**, for example salim123.pdf
6. **Submit the PDF file** as your final lab submission on Blackboard.


## INVESTIGATION 1: USING IF-ELSE AND input() FUNCTION
An IF statement is a decision statement that executes or does not execute a section of code based on whether the condition is True or False.
In investigation 1 you will learn how to take input from user, and compare it with other values.

### Task1 - Simple if statement
**Objective:** Practice using if statements in Python to make decisions based on user input, including type conversion, relational operators, and Boolean conditions.

**Instructions**
- Open the file `task1.py` and fill in the comments section.
- Create a variable named `x` and store in it a value entered by the user using the `input()` function.
  - The prompt should clearly ask the user to enter a number, for example:
    ```python
    x = input("Please enter a number: ")
    ```
  - **Note:** The `input()` function always returns a value of type `str` (string), even if the user enters a number.
- Use the `type()` function to check the type of `x` and print the result. You will observe that the type of `x` is `str`.
- Convert `x` to an integer using the `int()` function and update the variable `x` using the statement:
  ```python
  x = int(x)
 - Write an if statement to check if x is greater than or equal to 6. If the condition is True, print:
   - x is greater than or equal to 6!
 - Write another if statement that uses both relational and Boolean operators to check if x is greater than or equal to 4 and less than 12.
   - If the condition is True, print an appropriate message (for example:"x is between 4 and 11 inclusive").
 - Run the script from terminal to verify the output. 
### Task2 - Using if-else statement
**Objective:** Practice decision-making in Python using the `if-else` statement to compare user input with a specific value.

**Instructions:**
- Create a new file `task2.py` and add the comment section at the top.
- Use the input() function and ask the user to enter a 4-digit integer. Save this value in the variable `num`. For example:
  ```python
      num = input("Enter a 4-digit number: ")
  ```
  - Write an `if-else` statement to check if the number is **exactly 1984**:  
  - If `True`, print:  
      ```
      George Orwell
      ```  
  - If `False`, print:  
      ```
      Not quite right!
      ```
 - Run the script from terminal to verify the output. 


### Task3 - String comparison
**Objective:** Practice using `if`, `elif`, and `else` statements in Python to compare the length of strings entered by the user.

**Instructions**

- Create a new file `task3.py` and add the comment section at the top.
- Create two variables named `str1` and `str2` and assign them string values of your choice.
- Use the `len()` function to determine the length of each string.  
- Use `if`, `elif`, and `else` statements to compare the lengths of `str1` and `str2`:  
  - If `str1` is longer, print:  
    ```python
    str1 is longer than str2!
    ```  
  - If `str2` is longer, print:  
    ```python
    str2 is longer than str1!
    ```  
  - If they are equal in length, print:  
    ```python
    str1 and str2 are of equal length!
    ```
 - Run the script from terminal to verify the output. 

## INVESTIGATION 2: USING NESTED CONDITIONS
Using nested conditions are helpfull im multiple situations in python. Nested conditions are using statements like `if` and `else` multipule times on top of each other.These can be used when you have to narrow down specifics or doing more complex conditions. In investigation 2 you will learn how to use nested conditions.
-  Copy the following code snippet in Jupyter lab and run it to observe its output.
``` Python
x=3
if x < 6:
    if x >2: # this if is nested in the above if
        print("x is less than 6 and x is greater than 2.")
```

### Task4 - Income Tax Calculator with nested conditions
**Objective:** Practice using nested `if`, `elif`, and `else` statements in Python to apply conditional logic based on multiple variables.

![incomeTaxExample](https://github.com/user-attachments/assets/e7325ff1-a90f-445d-b119-06b95cc103c6)

**Instructions:**

- Create a new file `task4.py` and add the comment section at the top.
- Create a program that calculates tax based on the table in the image above.
- The script should include a variable `income`. The value of `income` should be entered by the user and should be a number (preferably in the thousands).
- Convert the input to an integer or float so it can be used in numeric comparisons.
- Include a variable `status`, prompt the user to enter either `"single"` or `"married"`.
- Use **nested** `if`, `elif`, and `else` statements to model the logic shown in the tax chart.  
- Use **relational operators** to compare `income` and `status` with the threshold values in the table.  
- Test your program with multiple different combinations of income and marital status to ensure it works correctly.


## INVESTIGATION 3: USING LOOPS
Loops are used in all programming languages to repeat code under certain conditions.  
A loop runs as long as its condition (expression) evaluates to `True`.  
When the condition becomes `False`, the program continues with the next line after the loop.

In Investigation 3, you will learn about the two main types of loops in Python:  
- `while` loop  
- `for` loop  


### Part A: while Loop:
In Python, a `while` loop is used to execute a block of statements repeatedly **while** a given condition is `True`.  
A `while` loop can use the same type of Boolean expressions found in `if` statements.  
While the condition remains `True`, all indented statements in the loop body will run repeatedly.  
When the condition becomes `False`, the loop stops.
**Note:** In Python, all statements indented by the same number of spaces after a control structure are considered part of the same block.

**Syntax:**
```python
while condition:
    statement(s)
```
**Key points:**
- Commonly used when you want to repeat statements until an event occurs (event-controlled loop).
- The loop must have a way to change the condition to avoid running forever.
- An iteration variable is often used in the condition and is updated inside the loop.
  
 ```python
count = 0  # iteration variable
while count != 5:  # condition (evaluates to True or False)
    print(count)   # loop body
    count = count + 1  # update the iteration variable

print('Loop has ended')  # runs after the condition becomes False
```

### Task5 - Understanding While Loops in Python
**Objective:** To explore counter-controlled and event-driven while loops in Python and understand common loop-related errors such as the off-by-one error.

**Instructions**
- Create a new file `task5.py` and add the comment section at the top.
- Copy the above code block in task5.py.
- Change the value of count to 1 and then run the program to see how many times the loop runs.
- Next change the while condition to `count < 5 ` and then run the program to see how many times the loop runs.
- Next change the condition to `count <= 5` and then run the program to see how many times the loop runs.
- What did you observe in all of the above examples when you change the value of loop variable or the expression. It is important that you are well aware of initial value of loop variable and the condition in the loop expression to know exactly how many times the loop will be executed.
- In the word document, under `Task5` write your reflections of this task.


Next, we will do a more complex but really useful example.
In Python, we often use while loop to see if the user entered the required value. We keep asking the user for a value until the user enters the correct value. This is a scenario-driven by an event rather than driven by a counter, because you do not know how many times the user will enter the incorrect value before the user enters the correct value. See the example below:

```Python
guess = 5
number = int(input("Guess what number less than 10 I am thinking of?"))
while number != guess:  # loop condition 
  print("incorrect guess, try again...")
  number = int(input("Guess what number less than 10 I am thinking off?")) # keep taking input from user until the user enters the correct guess.
print("You got it right!") # this statement will be executed when loop has terminated which will only happen when the user enters the number 5.

```

### Task6.py - Validating User Input with a While Loop
**Objective:** To use a while loop to repeatedly prompt the user for a 4-digit PIN until the correct value is entered.

**Instructions:**
- Create a new file `task6.py` and add the comment section at the top.
- Create a variable called `pin`. Use the `input()` function to ask the user to enter a 4-digit PIN.
- Use a while loop to keep asking for the PIN until the user enters the correct PIN `1234`.
- Add a validation check to ensure the user enters exactly 4 digits and that all characters are numeric.
- Your output should look like this:
```
Please type in your PIN: 0000
Incorrect...try again

Please type in your PIN: 199

Incorrect...enter a 4 digit number

Please type in your PIN: 1234
Correct PIN, You can enter!
```
Keep practicing, attempt this next exercise now!

### Task7 - Using break and continue in Loops
**Objective:** To practice using break and continue statements in Python loops to control flow based on user input.

**Instructions:**
- Create a new file `task7.py` and add the comment section at the top.
- Write a program that repeatedly prompts the user to input a number.
- Based on the input, the program should:
    -  **Negative Number**: Print "Invalid number." and prompt again (use continue).
    -  **Zero**: Print "Exiting ..." and terminate the loop (use break).
    - **Non-Negative Number**: Calculate and print the square root of the number
- **Sample output**: 
``` Python

Please type in a number: 9
3.0

Please type in a number: 1
1.0

Please type in a number: -9
Invalid number.

Please type in a number: 0
Exiting ...
```

### Part B: for Loop:
A for loop is used for iterating over a sequence (that could be either a list, a tuple, a dictionary, a set, or a string).
With the for loop we can execute a set of statements, once for each item in a list, tuple, set etc.
A very common example of for loop found in all text books is:

``` Python
fruits = ["apple", "banana", "cherry", "date"]

# Use a for loop to iterate over the list
for fruit in fruits:
    print(fruit)
```
for loop is commonly used with range functions. Here's another example using the range function to print numbers from 0  to 5.

``` Python
for i in range(5):
    print(i)
```
The range(5) function generates a sequence of numbers from 0 to 4 (inclusive of 0, exclusive of 5).


### Task8- Summing Even Numbers with a For Loop
**Objective:** To use a for loop and conditional logic to calculate the sum of all even numbers from 1 to 100 (inclusive).

**Instructions**
- Create a new file `task8.py` and add the comment section at the top.
- Write a Python program that.
   - Uses a for loop to iterate over the numbers from 1 to 100 (inclusive).
   - Checks if each number is even using the modulo operator (%).
   - Adds even numbers to a running total.
   - Prints the final sum after the loop ends.


## Lab 2 Sign-Off
- Submit a PDF named using your Seneca username, **<your-username>.pdf** on *Blackboard*.
- The document must include screenshots of the following scripts and their terminal output, clearly showing your GitHub username:
    - task1.py
    - task2.py
    - task3.py
    - task4.py
    - task5.py
    - task6.py
    - task7.py
    - task8.py

- Ensure the code and output are clearly readable. Screenshots should be high-resolution (minimum 800x600) and not blurry.
- Blurry or unreadable submissions will be returned for redo. Resubmissions will only be graded as "**Satisfactory**" with a grade of 0, provided the work is satisfactory. 
