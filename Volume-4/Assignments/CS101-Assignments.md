# CS101 — Assignments
## Introduction to Programming & Computational Thinking

**Total:** 5 assignments, biweekly, worth 25% of final grade (see Assessment Scheme in `Volume-2/CS101.md`)
**Format:** Auto-graded where possible (unit-test based), manually reviewed for style/documentation
**Submission:** Via GitHub repo (per CS102), one folder per assignment

---

## Assignment 1 — Fundamentals: Variables, Operators, Conditionals
**Due:** End of Week 4
**Covers:** Weeks 1–4

**Tasks:**
1. **Temperature Advisor** — Take a temperature (°C) as input. Output one of: "Freezing", "Cold", "Mild", "Warm", "Hot" based on defined ranges. Must use `if/elif/else`.
2. **Simple Interest Calculator** — Take principal, rate, and time as input; compute and print simple interest and total amount, formatted to 2 decimal places.
3. **Even/Odd/Zero Classifier** — Take an integer; classify it as zero, even, or odd, and also state whether it's positive or negative.
4. **Traceback Report** — Given 3 broken code snippets (provided), write a short explanation (1–2 sentences each) of what error occurs and why, then submit the fixed version.

**Grading Rubric:**
| Criterion | Weight |
|---|---|
| Correctness (passes test cases) | 60% |
| Handles edge cases (e.g., boundary temperatures, zero) | 20% |
| Code style & comments | 20% |

---

## Assignment 2 — Loops & Iteration
**Due:** End of Week 6
**Covers:** Weeks 5–6

**Tasks:**
1. **Prime Checker & Lister** — Write a function-free (loop-only, since functions aren't taught yet) script that lists all prime numbers up to N using nested loops.
2. **Number Pattern Printer** — Reproduce 3 given number/star patterns using nested loops (pyramid, inverted pyramid, diamond).
3. **String Analyzer** — Given a sentence, count vowels, consonants, digits, and spaces using a single `for` loop over characters.
4. **Guess the Number (Bounded)** — Simulate a number-guessing game where the program picks a fixed number (no `random` yet) and the user has a maximum of 5 attempts via a `while` loop with a counter.

**Grading Rubric:**
| Criterion | Weight |
|---|---|
| Correctness | 55% |
| Efficient use of loop constructs (no unnecessary repetition) | 20% |
| Edge case handling (N=0, N=1, empty string) | 15% |
| Code style & comments | 10% |

---

## Assignment 3 — Collections: Lists, Tuples, Dictionaries, Sets
**Due:** End of Week 9
**Covers:** Weeks 7–8

**Tasks:**
1. **Grade Book** — Given a list of student scores, compute class average, highest, lowest, and a sorted ranking — without using `sorted()` for the ranking part (manual sort logic), then compare with `sorted()`.
2. **Inventory Tracker** — Use a dictionary to model a small shop inventory (item → quantity). Support add stock, remove stock (with insufficient-stock check), and print full inventory.
3. **Duplicate & Unique Finder** — Given two lists, use sets to find: items only in list A, only in list B, and in both.
4. **Tuple-Based Coordinate Tool** — Store a list of (x, y) coordinate tuples; compute the distance between two selected points (introduces `math.sqrt`, first standard library use).

**Grading Rubric:**
| Criterion | Weight |
|---|---|
| Correctness | 55% |
| Appropriate data structure choice (e.g., dict vs list justified in comments) | 20% |
| Edge cases (empty inventory, insufficient stock) | 15% |
| Code style & comments | 10% |

---

## Assignment 4 — Functions & Recursion
**Due:** End of Week 11
**Covers:** Weeks 9–10

**Tasks:**
1. **Function Library** — Implement and unit-test: `is_palindrome(s)`, `gcd(a, b)` (iterative), `flatten(list_of_lists)`.
2. **Recursive Toolkit** — Implement recursively: `factorial(n)`, `power(base, exp)`, `sum_digits(n)`. Include a comment stating the base case for each.
3. **Refactor Challenge** — Take Assignment 3's Grade Book and refactor all logic into functions (`compute_average()`, `find_extremes()`, `rank_students()`) with docstrings.
4. **Scope Puzzle** — Given 3 short snippets involving global/local scope conflicts, predict the output (written answer) before running, then verify.

**Grading Rubric:**
| Criterion | Weight |
|---|---|
| Correctness (unit tests) | 50% |
| Proper use of parameters/return values (no unnecessary globals) | 20% |
| Recursion correctness (proper base case, no infinite recursion) | 20% |
| Docstrings & style | 10% |

---

## Assignment 5 — File I/O, Exceptions & Integration
**Due:** End of Week 13
**Covers:** Weeks 11–13 (cumulative — may draw on any prior week)

**Tasks:**
1. **Persistent Grade Book** — Extend Assignment 3/4's Grade Book to save to and load from a text or CSV-like file, using proper `with open(...)` context managers.
2. **Safe Calculator** — Build a calculator that handles division by zero, invalid input (non-numeric), and invalid operator, using `try/except` for each distinct failure mode.
3. **Log Analyzer** — Given a provided log `.txt` file, count how many lines match each of 3 given keywords, handling the case where the file might not exist.
4. **Cumulative Mini-Challenge** — One integrative problem combining functions + recursion + file I/O + exception handling (e.g., a recursive directory-style word-count tool reading from a nested text structure represented as a dict).

**Grading Rubric:**
| Criterion | Weight |
|---|---|
| Correctness | 45% |
| Proper exception handling (specific except clauses, not bare `except:`) | 25% |
| File handling correctness (context managers, no resource leaks) | 15% |
| Code style, docstrings, and cumulative integration quality | 15% |

---

## General Academic Integrity Note (applies to all 5 assignments)

- Assignments are individual work. Discussing approach with peers is allowed; sharing code is not.
- Auto-graded test cases are a necessary but not sufficient condition for full marks — style and edge-case handling are manually reviewed.
- Late submission policy follows the program-wide Academic Regulations (`Volume-1/02-Academic-Regulations.md` — not yet finalized).
