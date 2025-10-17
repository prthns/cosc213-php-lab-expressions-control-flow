Course: COSC 213
Lab Folder: /lab4/
Lab Title: Lab 6
Author: Ralph Juliano, Christy VK, Tatsuki Sugawara 
Date: October 2025

Course: COSC 213
Author: Ralph Juliano

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

Part 1 — Expressions
Demonstrates PHP arithmetic, concatenation, comparison (== vs ===), ternary, and null-coalescing operators.
Part 2 — Branching
Uses if, elseif, else, switch, and match to create conditional logic based on query parameters.
Part 3 — Loops
Shows for, while, do...while, and foreach loops with examples like summing numbers and FizzBuzz.
Part 4 — Grade Form
A web form that accepts a score, validates input, and displays the corresponding letter grade dynamically.
Part 5 — Student Toolkit
An interactive web tool with three views:

Times: Displays the current time and next 5 minutes.

Table: Generates a 10×10 multiplication table.

Stats: Analyzes comma-separated integers for count, sum, min, max, and average.

Equality Operators: == vs ===
== checks for loose equality, converting types if necessary.
Example: "5" == 5 → true
=== checks for strict equality, requiring both value and type to match.
Example: "5" === 5 → false
Always prefer === to avoid unexpected results caused by type conversion.

Example URLs
?score=85 → Displays grade B
?view=times → Shows current and next 5 minutes
?view=table → Displays multiplication table
?view=stats&nums=1,5,9,2 → Shows count, sum, min, max, and average

Notes
Include screenshots of:
Each PHP file’s output
Grade form results (valid and invalid inputs)
Toolkit pages for all views