Course: COSC 213 -Lab6

Lab Folder: /lab4/

Lab Title: Lab 6

Instructor: Christina Mjema

Author: Christy Vattatharakooran Kunjachan
Author: Ralph Juliano
Author: Tatsuki Sugawara


Date: 19 October 2025

Overview
This lab demonstrates core PHP programming concepts such as expressions, branching (conditional statements), and loops. The final part combines all concepts into a small “Student Toolkit” web application that dynamically renders different sections based on user input.

Folder Structure
lab4/
  01_expressions.php
  02_branching.php
  03_loops.php
  04_grade_form/
      index.php
  05_toolkit/
      index.php
  README.md

How to Run

Open a terminal or command prompt in the lab4 folder.
Start a PHP server using:
php -S localhost:8000

Open your browser and visit:
http://localhost:8000/01_expressions.php

http://localhost:8000/02_branching.php?role=editor&day=Sun&code=404

http://localhost:8000/03_loops.php

http://localhost:8000/04_grade_form/

http://localhost:8000/05_toolkit/

Summary of Parts

## Part 1 — Expressions

Demonstrates PHP arithmetic, concatenation, comparison (== vs ===), ternary, and null-coalescing operators.

Checklist.

  Equality Operators: == vs ===
  == checks for loose equality, converting types if necessary.
  Example: "5" == 5 → true
  === checks for strict equality, requiring both value and type to match.
  Example: "5" === 5 → false
  Always prefer === to avoid unexpected results caused by type conversion.

-- Sample Input/ Output --

sum=13 prod=30 a=15
14
20
Hello Ada
Hello Ada
bool(true)
bool(false)
Entry allowed
Result: Fail/NoScore
"5cats" + 1 = 6


## Part 2 — Branching

Uses if, elseif, else, switch, and match to create conditional logic based on query parameters.

-- Sample URL / Output--

/02_branching.php?role=editor&day=Sun&code=404

Welcome, admin
Back to work
OKish
404 => Not Found



## Part 3 — Loops
Shows for, while, do...while, and foreach loops with examples like summing numbers and FizzBuzz.

--Sample Output -- 

7 14 21 28 35 42 49 56 63 70
First N where sum>100 is 15, sum 105
do ...while ran 1 time(s) Subtotal (skip<1): 12.7
1 2 Fizz 4 Buzz Fizz 7 8 Fizz Buzz 11 Fizz 14 FizzBuzz 16 17 Fizz 19 
Buzz Fizz 22 23 Fizz Buzz 26 Fizz 28 29 FizzBuzz


## Part 4 — Grade Form
A web form that accepts a score, validates input, and displays the corresponding letter grade dynamically.

-- Sample URL-- 
- /04_grade_form/?score=95 → A
- /04_grade_form/?score=82 → B
- /04_grade_form/?score=-1 → Invalid score  
- /04_grade_form/?score=hello → Invalid score

## Part 5 — Student Toolkit

An interactive web tool with three views:

Times: Displays the current time and next 5 minutes.

Table: Generates a 10×10 multiplication table.

Stats: Analyzes comma-separated integers for count, sum, min, max, and average.

 Running the page
1. From the lab4 folder, run the PHP server.
2. Open the browser and go to:
    `http://localhost:8000/05_toolkit/?view=times`  - Times View
    `http://localhost:8000/05_toolkit/?view=table`  - Table View
    `http://localhost:8000/05_toolkit/?view=stats&nums=1,2,3,10,-4` - Stats View

 Notes:
  - Navigating between views using the view parameter.
  - Preventing non-integer input on Stats view

 -- Sample URL and Output -- 

?score=85 → Displays grade B
?view=times → Shows current and next 5 minutes
?view=table → Displays multiplication table
?view=stats&nums=1,5,9,2 → Shows count, sum, min, max, and average

