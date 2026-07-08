---
title: Reconciliation Log
aliases:
  - Contradiction Tracker
  - Gap Analysis
tags:
  - wiki
  - qa
  - reconciliation
---

# ⚠️ Reconciliation Log

> [!abstract]
> Tracks contradictions, gaps, and stale information found across the vault. Updated during the ingestion pass and whenever new issues are discovered.

---

## 🔴 Open Issues

### 1. `.agents/workflows/exam-solver.md` File Found & Patched
- **Status:** ✅ Resolved
- **Details:** The file existed (previously missed by the initial scan). It has been patched: "midterm" → "final exam" and "academic English" → "academic Persian" (to match [[AGENTS.md]] language rule). The workflow logic is also synthesized in [[Exam-Solver Workflow]].

### 2. No Textbook Coverage for Chapters 10, 11, 12
- **Status:** ℹ️ Gap
- **Details:** The `textbook/` directory only contains Chapter 8 (`8.md`) and Chapter 9 sections (`9-1.md` through `9-problems.md`). There is no textbook material for [[Chapter 10 - Non-Inertial Reference Frames|Ch. 10]], [[Chapter 11 - Dynamics of Rigid Bodies|Ch. 11]], or [[Chapter 12 - Coupled Oscillations and Normal Modes|Ch. 12]].
- **Impact:** Students must rely solely on lecture notes for these chapters.
- **Action:** Consider adding textbook chapters if available.

### 3. Lecture Notes Formatting Inconsistency
- **Status:** ℹ️ Minor
- **Details:** Notes from Apr 25 and Apr 27 do not have standard `#` title headers (they start with prose text instead of `# Chapter X`). All other notes follow the `# Chapter X - Lecture: Date` pattern.
- **Action:** Consider patching those two files to add proper titles for consistency.

---

## 🟡 Observations & Notes

### 4. Professor vs. Textbook Notation
- **Details:** The textbook uses $f_{\alpha\beta}$ notation for internal forces (§9.1), while the lecture notes use $\vec{F}_{ij}$. The physics is identical; only notation differs.
- **Risk:** Low -- but students should be aware of both notations for the exam.

### 5. Falling Rope: Two Competing Models
- **Details:** The [[Note Apr 11, 2026|Apr 11 lecture]] presents two models for the falling rope:
  - **Model 1 (Free Fall):** $\ddot{x} = g$, energy NOT conserved, $T = 2Mg$ at full extension
  - **Model 2 (Energy Conservation):** Assumes continuous rope, energy IS conserved
- **Resolution:** These are **not contradictory** -- they are different physical assumptions. The professor presented both to highlight how the choice of model affects the result. This is itself a pedagogical "trap."

### 6. Chapter 12 Notation Evolution
- **Details:** The early Ch. 12 lectures (Jun 1-13) use slightly different notation than the later ones (Jun 20-29). The core algorithm is the same, but the matrix notation $\{m\}$ vs $\{A\}$ stabilizes in the later lectures.
- **Action:** Use the [[Jun 20 - Normal Coordinate Algorithm|Jun 20 lecture]] as the canonical reference for the algorithm.

---

## 🟢 Resolved

### 1. `.agents/workflows/exam-solver.md` Found & Patched ({{date}})
- File existed but was missed in initial scan. Patched "midterm" → "final exam" and language → Persian.

### 2. "Midterm" → "Final Exam" Sweep ({{date}})
- All occurrences of "midterm" across the vault (README.md, exam-solver.md) updated to "final exam" since the midterm is over.

---

## 🔗 Related
- [[Brain-Map]]
- [[AGENTS.md]]
- [[Exam-Solver Workflow]]
