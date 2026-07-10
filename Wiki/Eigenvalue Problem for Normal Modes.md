---
title: Eigenvalue Problem for Normal Modes
aliases:
  - Secular Equation
  - Normal Mode Algorithm
  - Characteristic Equation
tags:
  - method
  - mechanics
  - linear-algebra
  - oscillations
---

# Eigenvalue Problem for Normal Modes

> [!summary] The Algorithm
> Finding the normal modes of any coupled oscillator system reduces to a **generalized eigenvalue problem**. This is the single most important algorithm for the final stretch of the course ([[Chapter 12 - Coupled Oscillations and Normal Modes|Ch. 12]]).

---

## 🔑 The Step-by-Step Algorithm

### Step 1: Write $T$ and $U$ in matrix form
From the [[Lagrangian Mechanics|Lagrangian]], identify the **mass matrix** $\{m\}$ and the **stiffness matrix** $\{A\}$:

$$T = \frac{1}{2} \sum_{jk} m_{jk} \dot{q}_j \dot{q}_k, \qquad U = \frac{1}{2} \sum_{jk} A_{jk} q_j q_k$$

### Step 2: Solve the Secular Determinant
$$|A - \omega^2 m| = 0$$

This yields the **normal frequencies** $\omega_1, \omega_2, \ldots, \omega_n$.

### Step 3: Find Eigenvectors (Mode Shapes)
For each $\omega_r$, solve:
$$\sum_j (A_{jk} - \omega_r^2\, m_{jk})\, a_{jr} = 0$$

### Step 4: Handle Degeneracy (if any)
If $\omega_r = \omega_s$ (degenerate), use **orthogonality** and **normalization** constraints. Make an arbitrary choice to fix the basis. See [[Note Jun 29, 2026|Jun 29]].

### Step 5: Normalize
Ensure eigenvectors satisfy:
$$\vec{a}_r^T \cdot \{m\} \cdot \vec{a}_s = \delta_{rs}$$

### Step 6: Construct Normal Coordinates
$$q_j(t) = \sum_r a_{jr}\, \eta_r(t), \qquad \ddot{\eta}_r + \omega_r^2\, \eta_r = 0$$

---

## 📚 Where It's Taught

| Lecture | Focus |
|---------|-------|
| [[Note Jun 1, 2026|Jun 1]] | Introduction with 2 pendulums |
| [[Note Jun 8, 2026|Jun 8]] | Generalized formulation |
| [[Note Jun 13, 2026|Jun 13]] | Orthogonality proof |
| [[Note Jun 20, 2026|Jun 20]] | The exam-ready checklist |
| [[Note Jun 27, 2026|Jun 27]] | 3-body application |
| [[Note Jun 29, 2026|Jun 29]] | Degeneracy + loaded string |

---

> [!tip] Exam Tip
> Memorize this 6-step algorithm cold. Every Chapter 12 problem follows it. The [[Exam-Solver Workflow]] is built around it.

---

## 🔗 Related

- [[Chapter 12 - Coupled Oscillations and Normal Modes]]
- [[Lagrangian Mechanics]]
- [[Exam-Solver Workflow]]
