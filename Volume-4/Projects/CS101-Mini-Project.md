# CS101 — Mini Project Specification
## Introduction to Programming & Computational Thinking

**Weight:** 20% of final course grade
**Duration:** Weeks 14–15 (with informal planning encouraged from Week 12 onward)
**Type:** Individual project
**Prerequisite Skills Required:** All Weeks 1–13 content; basic Git/GitHub submission (per CS102)

---

## Purpose

The mini project is the first point in the curriculum where a student must independently plan, build, and document a complete program end-to-end — without weekly scaffolding. It exists to validate that CS101's learning outcomes (LO1–LO5) have been internalized as a connected skill set, not as isolated weekly exercises.

---

## Mandatory Technical Requirements

Every project, regardless of theme, must demonstrate:

| Requirement | Where It's Assessed |
|---|---|
| At least 3 functions, each with a docstring | Code review |
| At least one loop (`for` or `while`) used meaningfully | Code review |
| At least one conditional branch with 2+ outcomes | Code review |
| File I/O (read and/or write) for persistence | Functional test |
| At least one `try/except` block handling a real failure case | Functional test |
| No bare `except:` clauses | Code review |
| PEP 8–consistent style (naming, spacing) | Code review |
| A README explaining what the program does and how to run it | Documentation check |

---

## Approved Project Themes

Students choose **one**:

### Option A — Text-Based Adventure Game
A small choice-driven game with at least 3 distinct rooms/scenes, an inventory system (list or dict), and a win/lose condition. Game state should save/load via file I/O so a player can resume.

### Option B — Unit & Currency Converter Suite
A menu-driven tool converting between at least 3 unit categories (e.g., length, temperature, currency using fixed rates). Must log conversion history to a file and allow reviewing past conversions.

### Option C — Personal Contact Book
An extension of Lab 9/12's contact book: add, search, update, delete contacts; persistent storage in a file; input validation (e.g., reject empty names, invalid phone formats) via exception handling.

### Option D — To-Do List Manager
Add/complete/delete tasks with priority levels; persistent storage; summary report (e.g., "3 pending, 2 completed") generated using loop-based aggregation.

*(Instructor may approve an alternative theme if it meets all Mandatory Technical Requirements — proposal due by Week 12.)*

---

## Project Milestones

| Milestone | Week | Deliverable |
|---|---|---|
| M1 — Proposal | 12 (informal) / 14 (formal) | One-paragraph description + which requirements map to which planned functions (pseudocode-level plan) |
| M2 — Working Draft | 14 (lab session) | Core logic functional, even if incomplete; TA check-in for early feedback |
| M3 — Final Submission | 15 | Complete program, README, committed to GitHub |

---

## Submission Requirements

- GitHub repository (personal, per CS102 skills) containing:
  - Main `.py` file(s)
  - `README.md` with: project description, how to run it, example usage, list of mandatory requirements and where each is implemented (self-audit table)
  - Sample data file (if applicable) demonstrating persistence
- Commit history should show incremental progress (not one single commit) — reflects Git workflow habits from CS102, lightly graded under "process."

---

## Assessment Rubric

| Criterion | Weight |
|---|---|
| Functional correctness (program runs, meets chosen theme's core behavior) | 35% |
| Mandatory technical requirements met (table above) | 30% |
| Code quality: structure, naming, docstrings, PEP 8 | 15% |
| README & documentation clarity | 10% |
| Git process (incremental commits, meaningful messages) | 10% |

**Note:** This project is explicitly *not* graded on visual polish or feature scope — a small, correct, well-documented program outperforms a large, buggy, undocumented one.

---

## Common Pitfalls (Instructor Guidance / Student-Facing Advice)

- Starting to code before writing the M1 plan — leads to unstructured, hard-to-debug programs.
- Cramming all logic into `main()` instead of using multiple small functions.
- Skipping exception handling until the end (should be designed alongside the "happy path," not bolted on).
- Forgetting file I/O persistence until the last moment — test save/load early.

---

## Future Connections

- This project's structure (functions, docstrings, exception handling, README) is the **minimum professional baseline** expected in every subsequent course's projects, starting with CS103's lab project and formalized further in SE201 (Software Engineering Principles, Semester 4).
- The Git submission workflow here is a lightweight version of what becomes mandatory practice in PR301 (Semester Project I, Semester 6) and the Capstone (PR401/PR402, Semester 8).
