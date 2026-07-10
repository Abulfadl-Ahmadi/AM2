---
title: Lagrangian Mechanics
aliases:
  - Lagrangian
  - Lagrange's Equations
  - Principle of Least Action
tags:
  - method
  - mechanics
  - lagrangian
  - foundational
---

# Lagrangian Mechanics

> [!summary] The Unifying Framework
> The Lagrangian formulation ($L = T - V$) is the backbone of the entire AM II course. It unifies all five chapters under a single variational principle: **Hamilton's Principle of Least Action**.

---

## 🔑 The Core Idea

$$\delta \int L \, dt = 0 \quad \Longrightarrow \quad \frac{d}{dt}\frac{\partial L}{\partial \dot{q}_i} - \frac{\partial L}{\partial q_i} = 0$$

Instead of forces (Newton), we work with **generalized coordinates** $q_i$, **kinetic energy** $T$, and **potential energy** $V$.

---

## 📚 Usage Across This Course

| Chapter | How Lagrangian Is Used |
|---------|----------------------|
| [[Chapter 8 - Central-Force Motion|Ch. 8]] | Two-body -> one-body via $L = \frac{1}{2}\mu\dot{r}^2 - U(r)$ |
| [[Chapter 9 - Dynamics of a System of Particles|Ch. 9]] | Conservation laws from cyclic coordinates (Noether) |
| [[Chapter 10 - Non-Inertial Reference Frames|Ch. 10]] | Lagrangian in rotating frames yields fictitious forces naturally |
| [[Chapter 11 - Dynamics of Rigid Bodies|Ch. 11]] | Rotational kinetic energy from the inertia tensor |
| [[Chapter 12 - Coupled Oscillations and Normal Modes|Ch. 12]] | $T$ and $U$ matrices for small oscillations come directly from $L$ |

---

## 🔗 Related

- [[Reduced Mass Method]] -- Applied Lagrangian technique
- [[Eigenvalue Problem for Normal Modes]] -- Linearized Lagrangian
- [[Exam-Solver Workflow]] -- Always starts from the Lagrangian
