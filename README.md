<div align="center">

<h1>SRT111 Lab 2 - Fall 2026</h1>

<strong>Prepared by:</strong> Tiayyba Riaz  
<strong>Total Marks: 10 </strong>  
<strong>Percentage Towards Final Grade: 2% </strong>  

</div>
In this lab, you will design, implement, and test Python programs that use decision-making and iteration to solve simple problems.

The lab is divided into two components:
- **Part A: In-Class Lab** (must be completed during the scheduled lab period and demonstrated to the professor for grading).
- **Part B: Take-Home Lab** (must be completed independently after class using a local installation of VS Code).

  
This lab focuses on the following Python concepts:
- `if`, `elif`, and `else` statements
- Nested conditional statements
- Input validation
- `while` loops
- `break` and `continue`
- `for` loops and accumulation patterns
  
## Academic Integrity and Use of AI

This lab is intended to assess your individual understanding of Python programming.
You may use AI tools (e.g., ChatGPT, Copilot, Gemini) to help explain concepts, syntax, or error messages. However, all submitted code must be your own work, and you must be able to explain your solution if asked by the professor.

Submitting copied, shared, or AI-generated solutions as your own work may result in a grade of zero and may be handled according to the College Academic Integrity Policy.

# Lab Objectives
By the end of this lab, you will be able to:
- Accept, process, and validate user input.
- Use conditional statements (`if`, `elif`, `else`) to make decisions.
- Implement `while` and `for` loops to solve programming problems.
- Use `break` and `continue` to control loop execution.
- Document and submit program output using screenshots and a PDF report.
  
## Submission Instructions

### Part A: In-Class Lab
- Complete all assigned in-class tasks during your scheduled lab.
- Demonstrate your completed work to the professor before leaving the lab.
- The professor may ask you to explain portions of your code.
- No PDF submission is required for Part A unless otherwise instructed.
- Each task carries 1.25 marks.

### Part B: Take-Home Lab

For each task:
1. Create and run the required Python script in VS Code.  
3. Take a screenshot that clearly shows:  
   - The code in the editor.  
   - The program output in the terminal.
   - Your Seneca username visible in the terminal.
4. Insert the screenshots into a Word document under under the appropriate task heading.  
5. Answer any reflection questions included in the lab.
6. Convert the Word document to PDF.  Name the PDF file using your Seneca usernmae `yourusername.pdf`.
7. Submit the PDF to Blackboard.
8. Each task carries 1.25 marks.

 ## Required File Header
For every Python file submitted in this lab (task1.py, task2.py, etc.), include the following comment block at the top of the file:
```Python
# Author: Your Name
# Date: YYYY-MM-DD
# Purpose: Brief description of what the program does.
# Usage: python ./task1.py
```
Update the Purpose and Usage lines appropriately for each task.

---
# Part A - In-Class Lab [50% marks]

### Task1 - Simple if statement
**Objective:** Practice using if statements in Python to make decisions based on user input, including type conversion, relational operators, and Boolean conditions.

An IF statement is a decision statement that executes or does not execute a section of code based on whether the condition is True or False.

**Instructions**
- Create a file named `task1.py`.
- Using `input()`, ask the user to enter a number and store it in a variable named `number`.
  ```python
  x = input("Please enter a number: ")
  ```
- Use the `type()` function to display the type of the value entered. Observe that `input()` always returns a string (`str`).
- Convert `number` to an integer using:
  ```python
   number = int(number)
  ```
- Write an if statement to check if x is greater than or equal to 6. If the condition is True, print:
  ``` text
  x is greater than or equal to 6!
  ```
- Write a second `if` statement that checks whether `number` is greater than or equal to `4` and less than `12`. If the condition is True, print:
  ``` text
  number is between 4 and 11
  ```
- Run the program from the terminal and verify the output.

### Task2 - Using if-else statement
**Objective:** Practice using an `if-else` statement to compare user input with a specific value.

**Instructions:**
- Create a new file named `task2.py`.
- Use the `input()` function to ask the user to enter a number and store it in a variable named `num`.
  ```python
    num = int(input("Enter a number: "))
  ```
- Write an `if-else` statement to check whether `num` is equal to `1984`.  
  - If `True`, print:  
    ``` text
    George Orwell
    ```  
  - Otherwise, print:  
    ```text
    Not quite right!
    ```
 - Run the program from the terminal and verify the output. 


### Task3 - String comparison
**Objective:** Practice using `if`, `elif`, and `else` statements to compare the lengths of two strings.

**Instructions**

- Create a new file `task3.py`.
- Use the `input()` function to ask the user to enter two strings and store them in variables named `str1` and `str2`.
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


### Task4 - Income Tax Calculator with nested conditions
**Objective:** Practice using nested `if`, `elif`, and `else` statements to make decisions based on more than one condition.

![incomeTaxExample](https://github.com/user-attachments/assets/e7325ff1-a90f-445d-b119-06b95cc103c6)

**Instructions:**

- Create a new file `task4.py`.
- Prompt the user to enter:
  - their annual income
  - their marital status (single or married)
- Use nested if, elif, and else statements to determine the appropriate tax rate from the table provided. If the table does not render properly, please use the table from slides of week3.  
- Display the tax rate that applies to the user.  
- Test your program using:
  - at least one single taxpayer
  - at least one married taxpayer
  - incomes from different tax brackets

# Part B - Take-Home Lab [50% marks]
Complete the following tasks independently after the scheduled lab using VS Code.
For each task:
- take screenshots showing both your code and program output.
- Insert the screenshots into your submission document under the appropriate task heading

Failure to include your username in the terminal screenshot may result in a grade of zero for that task.
Once you complete all the tasks, push your work to GitHub.

The tasks in this section focus on loop constructs, input validation, and loop control techniques in Python.

### Task5 - Exploring While Loops
**Objective:** Understand how the starting value and loop condition affect the number of iterations in a `while` loop.

**Instructions**
- Create a new file `task5.py`.
- Copy the following code into your file.
  ```python
    count = 0
    while count != 5:
        print(count)
        count = count + 1
    print("Loop has ended")
  ```
- Run the program and observe the output.
- Modify the program and run it again using each of the following changes.
  - Change `count = 0` to `count = 1`.
  - Change the condition to `count < 5`.
  - Change the condition to `count <= 5`.
- Take screenshots showing your code and the output for each version.
- In your Word document, answer the following reflection questions:
  - How did changing the starting value affect the output?
  - What was the difference between using `< 5` and `<= 5`?


### Task6 - Validating User Input with a While Loop
**Objective:** Use a `while` loop to repeatedly prompt the user until a valid PIN is entered.

**Instructions:**
- Create a new file `task6.py`.
- Ask the user to enter a 4-digit PIN and store the value in a variable named `pin`.
- Use a `while` loop to continue prompting the user until the correct PIN (`1234`) is entered.
- Before checking whether the PIN is correct, validate that:
  - the input contains exactly 4 characters
  - all characters are digits
- Display appropriate messages based on the input.
- Your output should look like this:
```
Please type in your PIN: 0000
Incorrect...try again

Please type in your PIN: 199
Incorrect...enter a 4 digit number

Please type in your PIN: 1234
Correct PIN, You can enter!
```
- Run the program and test it with several different inputs.
  
### Task7 - Using break and continue in Loops
**Objective:** To practice using break and continue statements in Python loops to control flow based on user input.

**Instructions:**
- Create a new file `task7.py`.
- Import the `math` module.
- Use a loop that repeatedly prompts the user to enter a number.
- Process the input as follows:
  - If the number is negative:
  - If the number is `0`:
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


### Task8 - Summing Even Numbers with a For Loop
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
