---
title: Chapter 8 - Central-Force Motion
aliases:
  - Central Force
  - Two-Body Problem
  - Kepler Problem
tags:
  - chapter
  - mechanics
  - central-force
---

# Chapter 8 — Central-Force Motion

> [!summary] Overview
> The study of two-body systems interacting via a force directed along the line connecting their centers. This is one of the few problems in mechanics that yields a **complete, exact analytical solution**. It applies to both celestial mechanics (planetary orbits) and microscopic interactions (Coulomb scattering).

---

## 🔑 Core Concepts

### The Reduced Mass Technique
The two-body problem is reduced to an equivalent one-body problem using the [[Reduced Mass Method]]. The Lagrangian becomes:

$$L = \frac{1}{2}\mu|\dot{\vec{r}}|^2 - U(r)$$

where $\mu = \frac{m_1 m_2}{m_1 + m_2}$ is the **reduced mass**.

- **See:** [[Reduced Mass Method]] for full derivation
- **Textbook:** [[Textbook Ch 8 - Central-Force Motion]] §8.2

### Conservation Laws
Because the potential depends only on $r$ (not angle), we get:
- **Conservation of angular momentum** → motion confined to a plane
- **Conservation of energy** → orbits are conic sections

These are direct consequences of [[Lagrangian Mechanics]] and Noether's theorem.

### Effective Potential
The radial equation is solved using the effective potential:
$$U_{eff}(r) = U(r) + \frac{\ell^2}{2\mu r^2}$$

### Kepler Orbits
For the inverse-square law ($U \propto -1/r$), the orbits are conic sections: ellipses, parabolas, and hyperbolas.

---

## 📖 Sources

| Source | File |
|--------|------|
| Textbook Ch. 8 | [[Textbook Ch 8 - Central-Force Motion]] (`textbook/8.md`) |
| Prerequisite for Ch. 9 | [[Chapter 9 - Dynamics of a System of Particles]] |

---

## 🔗 Related

- [[Reduced Mass Method]]
- [[Lagrangian Mechanics]]
- [[Chapter 9 - Dynamics of a System of Particles]] — Extends to $n$-body systems
