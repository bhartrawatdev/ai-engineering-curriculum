# Capstone Requirements
## PR401 — Capstone Project I & PR402 — Capstone Project II (Semester 8)

**Combined Weight:** 9 credits (PR401: 4, PR402: 5)
**Duration:** Full Semester 8 (two connected courses, not two separate projects)
**Type:** Individual or team (2–3 students, team option requires individual contribution logs)
**Prerequisite:** Completion of PR301 (Semester Project I, Semester 6) and at least 100 credits earned

---

## Purpose

The Capstone is the terminal validation of the entire program: every graduate attribute defined in `Volume-1/01-Program-Overview.md` (Section 2) must be demonstrable in one coherent, production-quality AI system built by the student. It is not a new-topic course — it introduces no new taught content, only integration, depth, and professional execution of everything from CS101 through AI404.

---

## Structural Relationship: PR401 vs. PR402

| | PR401 (Capstone I) | PR402 (Capstone II) |
|---|---|---|
| Focus | Proposal, research, design, core implementation | Full implementation, evaluation, deployment, defense |
| Weeks | 1–8 of Semester 8 | 9–16 of Semester 8 |
| Deliverable | Design document + working prototype | Production system + written report + oral defense |
| Grading | Formative (feeds into, doesn't finalize, final grade) | Summative (final capstone grade) |

PR401 and PR402 are **not independent** — a student cannot take PR402 without having completed PR401 in the same academic year, and the project topic must remain the same across both (topic changes require committee approval).

---

## Eligibility & Prerequisites

- Minimum 100 credits completed (out of 142 total) before PR401 registration.
- Mandatory completion (not just enrollment) of:
  - PR301 — Semester Project I
  - AI301–AI307 (Deep Learning, NLP, CV, RL, Vector DB foundations)
  - SE301, SE302 (MLOps + API Engineering foundations)
- Recommended (not mandatory) completion of AI401–AI404 (LLMs, RAG, Agents, Safety) — since Semester 7 runs concurrently with early capstone proposal work, exceptions are handled by the capstone committee.

---

## Capstone Committee Structure

- **Primary Advisor:** A faculty member from AI, CS, or SE department, chosen or assigned by Week 2 of PR401.
- **Second Reader:** Assigned by the department to provide independent evaluation at both PR401 design review and PR402 final defense.
- **Industry Mentor (Optional but Encouraged):** For teams pursuing an industry-sponsored or applied problem.

---

## Approved Capstone Categories

Every project must fall into one of the following, and must integrate at least **3 distinct courses'** worth of material (stated explicitly in the proposal):

1. **Applied AI Product** — An end-to-end AI-powered application (e.g., RAG-based domain assistant, agentic workflow tool) with real users or a realistic deployment target.
2. **Systems & Infrastructure** — MLOps pipelines, distributed training/inference systems, or AI platform tooling.
3. **Research Reproduction & Extension** — Reproducing a peer-reviewed paper's core result and extending it with a novel experiment or ablation.
4. **AI Safety & Evaluation** — Building an evaluation harness, red-teaming framework, or safety/alignment tooling for an existing model class.
5. **Domain-Specific AI System** — AI applied to a specific field (healthcare, finance, education, etc.) with attention to domain constraints and ethical considerations.

*(Category must be declared in the PR401 proposal; determines which rubric weighting variant applies — see Assessment section.)*

---

## PR401 — Capstone I Milestones (Weeks 1–8)

| Milestone | Week | Deliverable |
|---|---|---|
| M1 — Proposal | 2 | 2–3 page proposal: problem statement, category, related work (min. 5 references), success criteria |
| M2 — Design Review | 4 | System architecture document, data plan, evaluation plan, risk/ethics assessment |
| M3 — Prototype Checkpoint | 6 | Minimal working prototype demonstrating core technical feasibility (not full features) |
| M4 — PR401 Review | 8 | Committee review: prototype demo + design document; go/no-go decision to proceed into PR402 |

## PR402 — Capstone II Milestones (Weeks 9–16)

| Milestone | Week | Deliverable |
|---|---|---|
| M5 — Implementation Checkpoint | 11 | Core system functionally complete; interim progress report |
| M6 — Evaluation & Iteration | 13 | Formal evaluation results against M2's success criteria; iteration based on findings |
| M7 — Final Report Draft | 15 | Full written report (structure below) submitted for second-reader feedback |
| M8 — Final Defense | 16 | Oral defense + live demo + final report submission |

---

## Mandatory Technical & Professional Requirements

Every capstone, regardless of category, must demonstrate:

| Requirement | Rationale |
|---|---|
| Git-based version control with meaningful commit history across the full semester | SE/CS foundational habit, now at professional scale |
| Automated testing (unit and/or integration tests) | SE201, SE301 |
| A documented evaluation methodology with quantitative results | MA201, AI201, AI404 |
| Explicit discussion of limitations, failure cases, and ethical considerations | HU102, AI404 |
| A reproducibility artifact (README + setup instructions sufficient for an independent party to run the system) | SE301, professional practice |
| Deployment or a clear deployment plan (even if not fully live) | SE401 |

---

## Final Report Structure (Required for PR402 M7/M8)

1. Abstract
2. Introduction & Problem Statement
3. Related Work (min. 8 references, properly cited — connects to HU401 research methods)
4. System Design & Architecture
5. Implementation Details
6. Evaluation Methodology & Results
7. Discussion: Limitations, Failure Analysis, Ethical Considerations
8. Conclusion & Future Work
9. Individual Contribution Log (mandatory for team projects)
10. Appendices (code links, extended results, reproducibility instructions)

---

## Oral Defense Format (PR402, Week 16)

- **Duration:** 30 minutes per individual, 45 minutes per team (2–3 students)
- **Structure:** 15–20 min presentation + live demo, remainder committee Q&A
- **Panel:** Primary Advisor + Second Reader (+ Industry Mentor if applicable)
- **Individual accountability:** In team projects, each member must be able to answer questions about the *entire* system, not just their assigned component — verified through defense Q&A.

---

## Assessment Scheme (PR401 + PR402 Combined)

| Component | Weight | Assessed In |
|---|---|---|
| PR401 Design & Prototype (M1–M4) | 20% | PR401 |
| PR402 Implementation Quality & Evaluation Rigor | 30% | PR402 |
| Final Written Report | 25% | PR402 |
| Oral Defense | 15% | PR402 |
| Process: Git history, testing discipline, milestone adherence | 10% | Both |

**Passing threshold:** Minimum 40% overall AND a passing recommendation from both the Primary Advisor and Second Reader at the final defense. A student who fails the defense but passes all written components may be offered one re-defense opportunity within 4 weeks, per program-wide academic regulations (`Volume-1/02-Academic-Regulations.md` — pending finalization).

---

## Academic Integrity & Originality

- Capstone topics must be novel or a substantive extension of prior work — pure reproduction without extension only qualifies under Category 3 (Research Reproduction & Extension), and even then requires a clearly novel component.
- Use of AI coding assistants is permitted and expected (consistent with the program's "practical engineering" philosophy) but must be disclosed in the report's methodology section, with the student able to explain and defend every part of the system.
- Plagiarism in the written report (uncredited text or code) is handled per program-wide academic integrity policy and can result in capstone failure regardless of technical quality.

---

## Future Connections

- The capstone is the terminal integration point — it does not feed forward into another course, but its structure (design review → prototype → evaluation → defense) mirrors industry AI project lifecycles the graduate attributes (Section 2, Program Overview) are designed to prepare students for.
- Category 3 and 4 capstones (Research Reproduction, AI Safety & Evaluation) are the natural bridge for students considering graduate study or AI safety research careers.
