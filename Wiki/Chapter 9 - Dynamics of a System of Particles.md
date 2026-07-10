---
title: Chapter 9 - Dynamics of a System of Particles
aliases:
  - System of Particles
  - Many-Body Dynamics
  - Collisions and Scattering
tags:
  - chapter
  - mechanics
  - system-of-particles
  - collisions
---

# Chapter 9 — Dynamics of a System of Particles

> [!summary] Overview
> Extends mechanics from single particles to systems of $n$ particles. Covers **center of mass**, **linear and angular momentum conservation**, **energy of systems**, **collisions** (elastic & inelastic), **scattering cross sections**, and **rocket motion**.

---

## 🔑 Core Concepts

### 1. Linear Momentum & Center of Mass
- Total momentum: $\vec{P} = M\vec{V}_{CM}$
- Newton's 2nd Law for systems: $\frac{d\vec{P}}{dt} = \vec{F}^{ext}$
- Internal forces cancel by Newton's 3rd Law (weak form)
- **Conservation:** If $\vec{F}^{ext} = 0$, then $\vec{P} = \text{const}$

> [!warning] Trap: Directional Conservation
> Even when $\vec{F}^{ext} \neq 0$, if $\vec{F}^{ext} \cdot \hat{n} = 0$, momentum is conserved **along direction $\hat{n}$** only.

### 2. Angular Momentum
- Requires the **strong form** of Newton's 3rd Law (forces must be collinear)
- $\frac{d\vec{L}}{dt} = \vec{\tau}^{ext}$
- **Textbook:** [[Textbook Ch 9 - System of Particles]] §9.2–9.3

### 3. Energy of the System
- $E = K_{CM} + K_{internal} + U_{internal}$
- **Textbook:** §9.5

### 4. Collisions
- **Elastic:** Both momentum and kinetic energy conserved → [[Textbook Ch 9 - System of Particles|§9.7]]
- **Inelastic:** Only momentum conserved → §9.8
- Lab frame vs. CM frame transformations

### 5. Scattering Cross Sections
- Rutherford scattering, impact parameter, differential cross section
- $d\sigma/d\Omega$ → [[Note Apr 27, 2026|Apr 27]]
- **Textbook:** §9.9

### 6. Rocket Motion
- Variable-mass systems, thrust equation
- **Textbook:** §9.10–9.11

---

## 🧮 Key Example Problems

| Problem | Lectures | Key Insight |
|---------|----------|-------------|
| **Falling Rope** | [[Note Apr 11, 2026|Apr 11]] | Variable-mass; energy NOT conserved (inelastic bend) |
| **Scattering** | [[Note Apr 25, 2026|Apr 25]], [[Note Apr 27, 2026|Apr 27]] | Lab vs. CM frame |
| **Impulse & Sweet Spot** | [[Note Apr 25, 2026|Apr 25]] | Center of percussion |

---

## 📅 Lecture Notes

- [[Note Apr 4, 2026|Apr 4]]
- [[Note Apr 11, 2026|Apr 11]]
- [[Note Apr 13, 2026|Apr 13]]
- [[Note Apr 18, 2026|Apr 18]]
- [[Note Apr 20, 2026|Apr 20]]
- [[Note Apr 25, 2026|Apr 25]]
- [[Note Apr 27, 2026|Apr 27]]

## 📖 Textbook

- [[Textbook Ch 9 - System of Particles]] — Sections 9.1 through 9.11 + Problems

---

## 🔗 Related

- [[Chapter 8 - Central-Force Motion]] — Two-body special case
- [[Lagrangian Mechanics]] — Conservation laws via Noether's theorem
- [[Chapter 10 - Non-Inertial Reference Frames]] — Next chapter
