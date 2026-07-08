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
- $d\sigma/d\Omega$ → [[Apr 27 - Scattering Cross-Sections]]
- **Textbook:** §9.9

### 6. Rocket Motion
- Variable-mass systems, thrust equation
- **Textbook:** §9.10–9.11

---

## 🧮 Key Example Problems

| Problem | Lectures | Key Insight |
|---------|----------|-------------|
| **Falling Rope** | [[Apr 11 - Falling Rope & Energy]] | Variable-mass; energy NOT conserved (inelastic bend) |
| **Scattering** | [[Apr 25 - Scattering & Impulse]], [[Apr 27 - Scattering Cross-Sections]] | Lab vs. CM frame |
| **Impulse & Sweet Spot** | [[Apr 25 - Scattering & Impulse]] | Center of percussion |

---

## 📅 Lecture Notes

- [[Apr 4 - Dynamics of Particles Intro]]
- [[Apr 11 - Falling Rope & Energy]]
- [[Apr 13 - System Dynamics Cont.]]
- [[Apr 18 - CM & Angular Momentum]]
- [[Apr 20 - System Dynamics Cont.]]
- [[Apr 25 - Scattering & Impulse]]
- [[Apr 27 - Scattering Cross-Sections]]

## 📖 Textbook

- [[Textbook Ch 9 - System of Particles]] — Sections 9.1 through 9.11 + Problems

---

## 🔗 Related

- [[Chapter 8 - Central-Force Motion]] — Two-body special case
- [[Lagrangian Mechanics]] — Conservation laws via Noether's theorem
- [[Chapter 10 - Non-Inertial Reference Frames]] — Next chapter
