---
title: Chapter 12 - Coupled Oscillations and Normal Modes
aliases:
  - Coupled Oscillations
  - Normal Modes
  - Small Oscillations
  - Vibrations
tags:
  - chapter
  - mechanics
  - oscillations
  - eigenvalue
---

# Chapter 12 — Coupled Oscillations and Normal Modes

> [!summary] Overview
> Studies systems of coupled oscillators using the **eigenvalue problem**. The key insight is that any coupled system can be decomposed into **independent normal modes** — each a simple harmonic oscillator with its own characteristic frequency.

---

## 🔑 Core Concepts

### The Eigenvalue Problem
For a system with kinetic and potential energy matrices $\{m\}$ and $\{A\}$:

$$\sum_j (A_{jk} - \omega_r^2\, m_{jk})\, a_{jr} = 0$$

The normal frequencies $\omega_r$ are found from the **secular determinant**:

$$|A - \omega^2 m| = 0$$

- **See:** [[Eigenvalue Problem for Normal Modes]] for the complete algorithm

### Normal Coordinates
Each normal mode corresponds to an **independent coordinate** $q_r$ that decouples the equations of motion:

$$\ddot{q}_r + \omega_r^2\, q_r = 0$$

### Key Properties
- **Orthogonality:** $\vec{a}_r \cdot \{m\} \cdot \vec{a}_s = \delta_{rs}$
- **Normalization:** Eigenvectors normalized to unit length (when $m \to I$)
- **Degeneracy:** When two $\omega_r$ are equal, eigenvectors are not unique → free choice in a subspace

> [!danger] Trap: Degenerate Modes
> When $\omega_1 = \omega_2$, you have **fewer equations than unknowns**. You must use the orthogonality condition $\vec{a}_1 \cdot \vec{a}_2 = 0$ and make an **arbitrary choice** (e.g., set one component to zero) to lock in a specific basis. This is a classic exam trick!

---

## 🧮 Key Example Problems

| Problem | Lectures | Key Insight |
|---------|----------|-------------|
| **2 Coupled Pendulums** | [[Jun 1 - Coupled Oscillators]] | Symmetric & antisymmetric modes |
| **Weak Coupling & Beats** | [[Jun 6 - Weak Coupling & Beats]] | Energy transfer between oscillators |
| **3 Coupled Pendulums** | [[Jun 27 - 3 Coupled Pendulums]], [[Jun 29 - Degeneracy & Loaded String]] | Degeneracy handling |
| **Loaded String** | [[Jun 29 - Degeneracy & Loaded String]] | $n$ masses on a string → wave equation limit |
| **General Algorithm** | [[Jun 8 - Small Oscillations & Orthogonality]], [[Jun 13 - Mode Orthogonality & Normal Coords]], [[Jun 20 - Normal Coordinate Algorithm]] | The exam-ready procedure |

---

## 📅 Lecture Notes (Most Recent & Important)

- [[Jun 1 - Coupled Oscillators]]
- [[Jun 6 - Weak Coupling & Beats]]
- [[Jun 8 - Small Oscillations & Orthogonality]]
- [[Jun 13 - Mode Orthogonality & Normal Coords]]
- [[Jun 20 - Normal Coordinate Algorithm]]
- [[Jun 27 - 3 Coupled Pendulums]]
- [[Jun 29 - Degeneracy & Loaded String]]

---

## 🔗 Related

- [[Eigenvalue Problem for Normal Modes]] — The mathematical method
- [[Chapter 11 - Dynamics of Rigid Bodies]] — Inertia tensor uses similar diagonalization
- [[Lagrangian Mechanics]] — Foundation: $T$ and $U$ come from the Lagrangian

## 📖 Textbook Reference

- [[Textbook Ch 12 - Coupled Oscillations and Normal Modes]] (`textbook/12-1.md` - `textbook/12-problems.md`)
