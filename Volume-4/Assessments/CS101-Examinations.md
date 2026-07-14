# CS101 — Examinations
## Introduction to Programming & Computational Thinking

**Components:** Midterm Exam (15% of final grade) + Final Exam (20% of final grade)
**Format:** Closed-book (no internet/AI tools), paper-based or locked-environment digital, per program-wide exam policy (`Volume-1/02-Academic-Regulations.md` — pending finalization)

---

## Midterm Exam

**Timing:** End of Week 7 (after Strings, before Lists/Dicts)
**Duration:** 90 minutes
**Coverage:** Weeks 1–6 (Computation basics → Strings)
**Weight:** 15% of final course grade

### Structure

| Section | Format | Weight | Topics Covered |
|---|---|---|---|
| A — Conceptual | 8 short-answer questions (1–2 sentences each) | 20% | Computation basics, types, syntax vs. logical errors, operator precedence |
| B — Predict the Output | 6 code snippets, no running allowed | 25% | Operators, conditionals, loops, truthy/falsy behavior |
| C — Trace & Debug | 3 broken code snippets — identify + fix the bug | 25% | Conditionals, loops, string handling |
| D — Write a Program | 2 problems, write full working code by hand | 30% | Integrative: conditionals + loops + strings |

### Sample Question Types

- **Section A:** "Explain the difference between a syntax error and a logical error, with one example of each."
- **Section B:** Given `x = 5; y = "5"; print(x == y)` — what is the output and why?
- **Section C:** A provided `while` loop that never terminates — identify the missing update and fix it.
- **Section D:** "Write a program that takes a sentence and prints it with each word capitalized, without using `.title()`."

### Learning Outcomes Assessed
LO1 (correct implementation), LO2 (planning/tracing before running), LO3 (debugging).

---

## Final Exam

**Timing:** End of Week 15 (final exam period)
**Duration:** 150 minutes
**Coverage:** Cumulative, Weeks 1–13 (weighted toward Weeks 7–13, since Midterm already covered 1–6 in depth)
**Weight:** 20% of final course grade

### Structure

| Section | Format | Weight | Topics Covered |
|---|---|---|---|
| A — Conceptual | 10 short-answer questions | 15% | Full course, emphasis on functions, recursion, exceptions |
| B — Predict the Output | 8 code snippets | 20% | Lists/dicts/sets behavior, function scope, recursive calls |
| C — Trace & Debug | 4 broken snippets | 20% | Functions, recursion, file I/O, exception handling |
| D — Write a Program (Medium) | 2 problems | 25% | Functions + one data structure (list/dict) |
| E — Write a Program (Integrative) | 1 larger problem | 20% | Combines functions + recursion or loop + file I/O + exception handling — mirrors mini-project requirements at smaller scale |

### Sample Question Types

- **Section A:** "What is a base case in recursion, and what happens if a recursive function has no base case?"
- **Section B:** Given a recursive function call, trace and state the final return value.
- **Section C:** A provided function with a mutable default argument bug — identify and fix.
- **Section D:** "Write a function `word_frequency(text)` that returns a dictionary of word counts."
- **Section E:** "Write a program that reads a file of numbers (one per line), safely handles a possible missing file or invalid (non-numeric) line, and writes the sum and average to a new output file."

### Learning Outcomes Assessed
All of LO1–LO5, with Section E specifically validating LO5 (functions eliminating duplication) and LO4 (recursion) in an integrated context.

---

## Grading & Academic Integrity

- Exams are individually invigilated; no collaboration, notes, or AI/internet tools permitted (consistent with program-wide policy).
- Partial credit is awarded in Sections C–E for correct approach/logic even if the final code has minor syntax errors — CS101 exams assess computational thinking, not syntax memorization.
- Minimum 35% required on the Final Exam component specifically, regardless of overall course average, to pass CS101 (per the course's Assessment Scheme in `Volume-2/CS101.md`).

---

## Exam-to-Outcome Mapping (Summary)

| Learning Outcome | Midterm | Final |
|---|---|---|
| LO1 — Implement a spec correctly | ✅ | ✅ |
| LO2 — Decompose/plan before coding | ✅ | ✅ |
| LO3 — Identify and fix errors | ✅ | ✅ |
| LO4 — Recursive solution | — | ✅ |
| LO5 — Functions eliminate duplication | — | ✅ |

*(Recursion and functions are not yet taught by the Midterm's Week 1–6 cutoff, hence their absence there — this is intentional, not a gap.)*
