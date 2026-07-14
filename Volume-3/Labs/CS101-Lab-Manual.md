# CS101 — Laboratory Manual
## Introduction to Programming & Computational Thinking

**Format:** Weekly 2-hour lab sessions, aligned to CS101 lecture units (see `Volume-2/CS101.md`)
**Progression Model:** Guided (Weeks 1–4) → Scaffolded (Weeks 5–9) → Independent (Weeks 10–13) → Project (Weeks 14–15)
**Tooling:** Python 3.x, terminal, text editor/IDE (Git usage reinforced per CS102, not required until submission)

---

## Lab 1 — Environment & First Programs
**Aligned to:** Week 1

**Objectives:** Confirm environment setup; write and run first scripts.

**Exercises:**
1. Verify Python installation; run `python3 --version` in terminal.
2. Write a script that prints your name, program, and today's date.
3. Modify the script to take your name via `input()` and greet you back.
4. Deliberately introduce a syntax error, observe the traceback, fix it.

**Stretch Problem:** Write a script that prints a simple ASCII art shape using multiple `print()` statements.

**Submission:** Single `.py` file, no Git required yet (local submission via LMS/portal).

---

## Lab 2 — Variables & Types
**Aligned to:** Week 2

**Objectives:** Practice variable assignment, typing, and conversion.

**Exercises:**
1. Store your age, height (float), and student status (bool) in variables; print all three with labels.
2. Write a script that takes two numbers as string input and adds them correctly (requires casting).
3. Use `type()` to print the type of five different values; explain each in a comment.
4. Debug a provided broken script where a `TypeError` occurs due to missing casting.

**Stretch Problem:** Build a simple unit converter (Celsius → Fahrenheit) using `float()` casting and a formula.

---

## Lab 3 — Operators & Expressions
**Aligned to:** Week 3

**Objectives:** Apply arithmetic, comparison, and logical operators correctly.

**Exercises:**
1. Write expressions to compute area and perimeter of a rectangle from user input.
2. Predict-then-run: given 5 expressions with mixed operator precedence, predict output before running.
3. Write a script using `and`/`or`/`not` to check if a number is in a valid range.
4. Fix a script with an operator precedence bug (e.g., missing parentheses).

**Stretch Problem:** Implement a simple BMI calculator with a comparison-based category output (underweight/normal/overweight).

---

## Lab 4 — Conditionals
**Aligned to:** Week 4

**Objectives:** Build multi-branch decision logic.

**Exercises:**
1. Grade classifier: input a numeric score, output a letter grade using `if/elif/else`.
2. Leap year checker (requires nested/compound conditions).
3. Simple rock-paper-scissors outcome logic (two inputs, print winner).
4. Debug a provided script with an `=` vs `==` bug.

**Stretch Problem:** Build a basic triangle validator (given 3 side lengths, determine if valid and classify as equilateral/isosceles/scalene).

*(End of guided phase — Labs 5 onward are scaffolded: partial starter code provided, more blanks to fill independently.)*

---

## Lab 5 — Loops I (`while`)
**Aligned to:** Week 5 (part 1)

**Exercises:**
1. Number guessing game using `while` (fixed target, loop until correct).
2. Sum of digits of a number using `while` and modulo.
3. Input validation loop: keep asking until user enters a positive integer.
4. Debug an infinite loop (missing update to loop variable).

**Stretch Problem:** Simulate a basic ATM withdrawal loop (balance decreases, loop ends when balance insufficient or user quits).

---

## Lab 6 — Loops II (`for`, nested loops)
**Aligned to:** Week 5 (part 2)

**Exercises:**
1. Print a multiplication table (1–10) using nested `for` loops.
2. Sum and average of a series of `range()`-generated numbers.
3. Simple pattern printing (triangle of stars) using nested loops.
4. Count vowels in a sentence using a `for` loop over characters.

**Stretch Problem:** FizzBuzz (1–100) — classic but effective for reinforcing loop + conditional combination.

---

## Lab 7 — Strings
**Aligned to:** Week 6

**Exercises:**
1. Palindrome checker using slicing.
2. Word counter: count words in a sentence using `.split()`.
3. Simple Caesar cipher (shift letters by a fixed amount) — introduces character-code thinking.
4. Format a report line using f-strings from given variables.

**Stretch Problem:** Build a basic "Mad Libs" generator using `.format()` or f-strings and multiple `input()` calls.

---

## Lab 8 — Lists & Tuples
**Aligned to:** Week 7

**Exercises:**
1. Build a list of 5 numbers via input; compute sum, average, max, min manually (no built-ins first, then compare to `sum()`/`max()`/`min()`).
2. Remove duplicates from a list (without using `set()` — sets come next week).
3. Reverse a list manually using a loop, then compare to `.reverse()` and slicing `[::-1]`.
4. Simple to-do list manager: add/remove/view items using a list (in-memory only, no file I/O yet).

**Stretch Problem:** Implement a basic list-based matrix (list of lists) and print it in grid format — informal precursor to MA104 (Linear Algebra).

---

## Lab 9 — Dictionaries & Sets
**Aligned to:** Week 8

**Exercises:**
1. Build a simple contact book using a dictionary (name → phone number); support add/lookup/delete.
2. Word frequency counter using a dictionary.
3. Use sets to find common elements between two lists (intersection).
4. Compare performance conceptually: list membership check vs. set membership check (discussion, not benchmarking yet — that's CS202).

**Stretch Problem:** Extend the contact book to store multiple fields per contact (nested dictionary).

*(End of scaffolded phase — Labs 10 onward are independent: spec given, no starter code.)*

---

## Lab 10 — Functions I
**Aligned to:** Week 9

**Exercises:**
1. Refactor Lab 4's grade classifier into a function `get_grade(score)`.
2. Write a function library: `is_even()`, `is_prime()`, `factorial()` (iterative).
3. Refactor Lab 9's contact book operations into functions (`add_contact()`, `find_contact()`, etc.).
4. Demonstrate scope: write a script showing a variable shadowing bug and fix it.

**Stretch Problem:** Build a small "calculator" program where each operation is its own function, dispatched via conditionals.

---

## Lab 11 — Recursion
**Aligned to:** Week 10

**Exercises:**
1. Recursive factorial and compare to iterative version from Lab 10.
2. Recursive sum of a list.
3. Recursive digit sum of a number.
4. Trace and diagram the call stack (on paper/comment) for `factorial(5)`.

**Stretch Problem:** Recursive Fibonacci — implement, then discuss (in comments) why it becomes slow for larger `n` (informal setup for complexity analysis in CS202).

---

## Lab 12 — File I/O & Exceptions
**Aligned to:** Week 11

**Exercises:**
1. Write contact book data (Lab 9/10) to a text file; read it back on program start.
2. Handle `FileNotFoundError` gracefully when the file doesn't exist yet.
3. Wrap Lab 5's input validation loop with proper `try/except` instead of manual checks.
4. Build a simple log-writer: append timestamped messages to a file.

**Stretch Problem:** Build a persistent to-do list (Lab 8) that saves/loads from a file, surviving program restarts.

---

## Lab 13 — Debugging & Code Quality
**Aligned to:** Week 12–13

**Exercises:**
1. Debug clinic: 4 provided broken scripts (off-by-one, mutable default argument, wrong scope, type mismatch) — fix and annotate the bug in a comment.
2. Refactor a messy provided script to follow PEP 8 (naming, spacing, docstrings).
3. Add `assert`-based sanity checks to 2 functions from Lab 10's function library.
4. Peer review: exchange Lab 12 solutions with a classmate, leave 3 written comments each (first exposure to code review, formalized in SE201).

---

## Labs 14–15 — Mini-Project Work Sessions
**Aligned to:** Week 14–15

**Structure:**
- Session 1: Proposal + planning — pick from approved mini-project list (text game, unit converter, contact book, to-do app); write pseudocode/function breakdown before coding.
- Session 2: Implementation + instructor/TA check-ins; must demonstrate functions, a loop, a conditional branch, and file I/O (per course spec).

**Submission Requirements:**
- Single well-documented `.py` file (or small multi-file project)
- Docstrings on all functions
- Committed to a personal GitHub repo (first graded use of CS102 skills), README with usage instructions

---

## Lab Assessment Guidelines

| Component | Weight (within Lab Performance, 20% of course grade) |
|---|---|
| Weekly exercise completion & correctness | 60% |
| Stretch problem attempts | 15% |
| Code quality / style adherence (Weeks 9+) | 15% |
| Participation & debugging clinic engagement | 10% |
