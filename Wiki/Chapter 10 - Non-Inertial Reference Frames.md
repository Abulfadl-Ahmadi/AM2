---
title: Chapter 10 - Non-Inertial Reference Frames
aliases:
  - Non-Inertial Frames
  - Rotating Frames
  - Coriolis
  - Fictitious Forces
tags:
  - chapter
  - mechanics
  - non-inertial
---

# Chapter 10 — Motion in Non-Inertial Reference Frames

> [!summary] Overview
> Studies dynamics in **accelerating** and **rotating** reference frames. Introduces **fictitious (inertial) forces**: the Coriolis force, centrifugal force, and transverse (Euler) force.

---

## 🔑 Core Concepts

### Fictitious Forces in a Rotating Frame

| Force | Formula | Origin |
|-------|---------|--------|
| **Centrifugal** | $m\omega^2 r$ (outward) | Frame rotation |
| **Coriolis** | $-2m\vec{\omega} \times \vec{v}$ | Velocity in rotating frame |
| **Transverse (Euler)** | $-m\dot{\vec{\omega}} \times \vec{r}$ | Angular acceleration |

> [!warning] Trap: Coriolis Direction
> The Coriolis force is always **perpendicular** to both $\vec{\omega}$ and $\vec{v}$. In the Northern Hemisphere, it deflects moving objects to the **right**. Always use the right-hand rule carefully.

### Equation of Motion
$$m\vec{a}_{rot} = \vec{F}_{real} - m\vec{\omega} \times (\vec{\omega} \times \vec{r}) - 2m\vec{\omega} \times \vec{v}_{rot} - m\dot{\vec{\omega}} \times \vec{r}$$

### The Earth as a Non-Inertial Frame
- Coriolis effect on weather patterns, Foucault pendulum
- Effective gravity: $\vec{g}_{eff} = \vec{g} - \vec{\omega} \times (\vec{\omega} \times \vec{r})$

---

## 📅 Lecture Notes

- [[Note May 2, 2026|May 2]]
- [[Note May 4, 2026|May 4]]
- [[Note May 9, 2026|May 9]]

---

## 🔗 Related

- [[Chapter 11 - Dynamics of Rigid Bodies]] — Rotational dynamics extended
- [[Lagrangian Mechanics]] — Lagrangian formulation in non-inertial frames

## 📖 Textbook Reference

- [[Textbook Ch 10 - Non-Inertial Reference Frames]] (`textbook/10.1.md` - `textbook/10.4.md`)
