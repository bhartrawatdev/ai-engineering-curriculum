# Consistency Review — Semester 1
## Phase 10 Checkpoint

**Scope of Review:** All 6 Semester 1 courses (CS101, CS102, CS103, MA101, MA102, HU101), cross-referenced against the Program Overview (Phase 1) and each course's own "Where It Is Used Later" / "Future Connections" claims.

**Method:** Manual audit against four failure categories per the master prompt: missing prerequisites, duplicate topics, incorrect ordering, knowledge gaps.

---

## 1. Prerequisite Consistency

| Check | Result |
|---|---|
| Do all Semester 1 courses correctly have "None" as prerequisite? | ✅ Pass — correct, as Semester 1 is the program entry point |
| Are corequisites correctly declared? | ✅ Pass — CS101↔CS103, CS101↔CS102 all mutually consistent across files |
| Do any Semester 1 courses silently assume knowledge not yet taught? | ⚠️ **Minor issue found** — see 1a |

**1a — Minor Issue:** MA101 Week 1 assumes "pre-university algebra/trigonometry" and CS101 assumes no math background at all — this is fine individually, but neither course states this assumption *to the student* in a visible way (e.g., an admissions/placement note). **Recommendation:** Add a short "Assumed Incoming Knowledge" note to `01-Program-Overview.md` rather than repeating it in every course file — avoids duplication (see Section 2).

---

## 2. Duplicate Topic Check

| Topic | Appears In | Verdict |
|---|---|---|
| Debugging methodology | CS101 (Week 12), CS103 (shared labs) | ✅ Not a duplicate — CS103 explicitly shares CS101's lab manual by design, documented as intentional in CS103's spec. Fine as-is. |
| Git submission workflow | CS102 (Weeks 9–14), referenced in CS101/CS103 mini-project | ✅ Not a duplicate — CS102 *teaches* Git, CS101/CS103 *use* it for submission. Correct dependency direction. |
| README/documentation writing | CS101 (Mini Project spec), HU101 (Weeks 2–3) | ⚠️ **Overlap found** — see 2a |
| Proof/induction basics | MA102 only | ✅ No duplication — correctly isolated to MA102, referenced (not retaught) elsewhere |

**2a — Overlap Issue:** Both CS101's Mini Project spec and HU101 Weeks 2–3 teach README writing, and both use the *same* CS101 mini-project as the practice artifact. This is **not a redundancy bug** — it's intentional integration (HU101 explicitly frames itself as building the CS101 README into a graded artifact) — but it is not clearly cross-referenced in `Volume-2/CS101.md` itself. **Recommendation:** Add a one-line note in CS101's Mini Project spec pointing to HU101's involvement, so a reader of CS101 alone doesn't miss that this connection exists. Low priority, cosmetic fix.

---

## 3. Ordering Check

| Check | Result |
|---|---|
| Does any course require content from a course running *later* in the same semester? | ✅ Pass |
| Does the corequisite structure (CS101/CS102/CS103 running in parallel) create a chicken-and-egg problem? | ⚠️ **Issue found** — see 3a |

**3a — Ordering Issue (moderate):** CS101's Mini Project (Weeks 14–15) requires Git submission (per its Submission Requirements), and Git is taught in CS102 across **Weeks 9–14** — meaning Git branching/collaboration content (CS102 Week 11+) finishes in the *same* week the CS101 project is due. This is tight but not necessarily broken, since CS102 Week 9 (basic `git init/add/commit`) is sufficient for *simple* submission — full collaboration workflow isn't required for an individual mini-project. **However**, this dependency is currently implicit, not stated. **Recommendation:** Add an explicit note to CS101's Mini Project spec: "Git submission requires only basic local commit workflow (CS102 through Week 10); full PR/branching workflow is not required for this deliverable." This removes ambiguity for instructors and students alike.

---

## 4. Knowledge Gap Check

| Check | Result |
|---|---|
| Are there any concepts *used* in a Semester 1 course that are *not taught* anywhere in Semester 1 or assumed as prior knowledge? | ✅ Pass, with one note — see 4a |
| Do all "Future Connections" claims in each course file point to real, already-planned courses? | ✅ Pass — spot-checked against Phase 1's high-level course list (CS104/105, MA103/104, CS201/202, MA201, AI201, AI301, CS204, SE201, SE301, HU401, HU402, PR301, PR401/402 — all exist in the Phase 1 list) |

**4a — Note (not a blocker):** MA101 Week 12 introduces Riemann sums "conceptually" for definite integrals, but no course in Semester 1 or Semester 2 (per current Phase 1/2 scope) formally revisits numerical approximation methods until MA301 (Numerical Methods, Semester 5). This is a 4-semester gap between introduction and reinforcement. **Recommendation:** Not urgent — flag for awareness when MA103/MA104 (Semester 2) are specified in detail, to check whether a brief reinforcement fits naturally there. No action needed now.

---

## 5. Assessment Weight Sanity Check

*(Not explicitly requested by the master prompt's Phase 10 criteria, but included as a useful sanity check since 6 fully-specified courses now exist.)*

| Course | Sum of Assessment Weights |
|---|---|
| CS101 | 100% ✅ |
| CS102 | 100% ✅ |
| CS103 | 100% ✅ |
| MA101 | 100% ✅ |
| MA102 | 100% ✅ |
| HU101 | 100% ✅ |

All individual course assessment schemes correctly sum to 100%. No arithmetic errors found.

---

## Summary of Findings

| Severity | Count | Items |
|---|---|---|
| 🔴 Blocking | 0 | — |
| ⚠️ Moderate | 1 | 3a — Git/Mini-Project timing ambiguity |
| ⚠️ Minor | 1 | 2a — README overlap cross-reference missing |
| 📝 Note (no action) | 2 | 1a — assumed knowledge not stated at program level; 4a — long gap before numerical methods reinforcement |

**Overall verdict:** Semester 1 is structurally sound. No missing prerequisites, no true duplicate content, no broken ordering. The two flagged items are documentation clarity issues, not curriculum design flaws — they don't require redesigning anything, just adding cross-reference notes.

---

## Recommended Fixes (Optional, Low-Effort)

1. Add "Assumed Incoming Knowledge" note to `Volume-1/01-Program-Overview.md`.
2. Add one cross-reference line in CS101's Mini Project spec noting HU101's role in the README deliverable.
3. Add one clarifying line in CS101's Mini Project spec on the minimum Git competency required (Week 10 level, not full PR workflow).

None of these are blocking — they can be batched into a single small update whenever convenient, or done now if you'd prefer a clean baseline before moving to Semester 2.
