---
title: Chapter 11 - Dynamics of Rigid Bodies
aliases:
  - Rigid Body Dynamics
  - Moment of Inertia
  - Euler Angles
  - Gyroscope
tags:
  - chapter
  - mechanics
  - rigid-body
  - rotation
---

# Chapter 11 — Dynamics of Rigid Bodies

> [!summary] Overview
> The study of bodies whose constituent particles maintain fixed relative distances. Covers the **inertia tensor**, **Euler's equations of motion**, **Euler angles**, and the dynamics of **gyroscopes** and tops.

---

## 🔑 Core Concepts

### The Inertia Tensor
A $3 \times 3$ symmetric matrix that generalizes "moment of inertia" to 3D rotation:

$$I_{ij} = \int \rho(\vec{r})\left(\delta_{ij}r^2 - x_i x_j\right) d^3r$$

- **Principal axes:** Diagonalize the tensor → principal moments $I_1, I_2, I_3$
- **Parallel axis theorem** and **perpendicular axis theorem**

> [!warning] Trap: Tensor vs. Scalar
> The "moment of inertia" $I$ from introductory physics is just **one component** of the full inertia tensor. For a general 3D rotation, you must use the full tensor.

### Angular Momentum of a Rigid Body
$$\vec{L} = \mathbf{I} \cdot \vec{\omega}$$
$\vec{L}$ and $\vec{\omega}$ are **NOT** generally parallel (unless rotating about a principal axis)!

### Euler's Equations of Motion
$$I_1\dot{\omega}_1 - (I_2 - I_3)\omega_2\omega_3 = \tau_1$$
$$I_2\dot{\omega}_2 - (I_3 - I_1)\omega_3\omega_1 = \tau_2$$
$$I_3\dot{\omega}_3 - (I_1 - I_2)\omega_1\omega_2 = \tau_3$$

### Euler Angles
Three angles $(\phi, \theta, \psi)$ that parameterize the orientation of a rigid body:
- **Precession** $\phi$
- **Nutation** $\theta$
- **Spin** $\psi$

### Gyroscopes & Tops
- Torque-free precession
- Steady precession of a heavy symmetric top
- "Gyroscopic rigidity" — a spinning gyroscope resists changes to its axis

---

## 📅 Lecture Notes

- [[May 11 - Rigid Body Dynamics]]
- [[May 16 - Rigid Bodies Cont.]]
- [[May 18 - Rigid Bodies Cont.]]
- [[May 23 - Rigid Bodies Cont.]]
- [[May 25 - Rigid Bodies Cont.]]
- [[May 30 - Rigid Bodies Cont.]]

---

## 🔗 Related

- [[Chapter 10 - Non-Inertial Reference Frames]] — Prerequisite (rotating frames)
- [[Chapter 12 - Coupled Oscillations and Normal Modes]] — Small oscillations around equilibrium
- [[Lagrangian Mechanics]] — $L = T - V$ with rotational kinetic energy
