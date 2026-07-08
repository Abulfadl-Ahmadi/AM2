---
title: Reduced Mass Method
aliases:
  - Reduced Mass
  - One-Body Reduction
tags:
  - method
  - mechanics
  - central-force
  - two-body
---

# Reduced Mass Method

> [!summary] Two Bodies -> One Body
> A coordinate transformation that reduces the two-body problem to an equivalent one-body problem. Instead of tracking $r_1$ and $r_2$ separately, we track the center of mass $R$ and the relative coordinate $r = r_1 - r_2$.

---

## 🔑 Derivation

Given $m_1 r_1 + m_2 r_2 = 0$ (CM frame) and $r = r_1 - r_2$:

$$r_1 = \frac{m_2}{m_1 + m_2}\,r, \qquad r_2 = -\frac{m_1}{m_1 + m_2}\,r$$

Substituting into the Lagrangian:

$$L = \frac{1}{2}\mu|\dot{r}|^2 - U(r)$$

where the **reduced mass** is:

$$\boxed{\mu \equiv \frac{m_1 m_2}{m_1 + m_2}}$$

The problem is now a single particle of mass $\mu$ moving in potential $U(r)$.

---

## 📚 Where It Appears

- [[Chapter 8 - Central-Force Motion]] -- The foundational application
- [[Textbook Ch 8 - Central-Force Motion]] §8.2 -- Full derivation
- [[Chapter 9 - Dynamics of a System of Particles]] -- CM concept extended to $n$ bodies

---

## 🔗 Related

- [[Lagrangian Mechanics]]
- [[Chapter 8 - Central-Force Motion]]
