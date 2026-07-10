---
title: Effective Potential
category: concept
tags: [mechanics, orbital-dynamics, visualization]
sources: ["textbook/8.md"]
created: 2026-07-09T02:37:00
updated: 2026-07-09T02:37:00
base_confidence: 0.5
lifecycle: draft
tier: core
summary: A visualization tool combining physical potential energy with a "centrifugal" potential to simplify 2D orbital problems into 1D.
provenance: {extracted: 1.0, inferred: 0.0, ambiguous: 0.0}
relationships:
  - target: "[[concepts/Central-Force-Motion]]"
    type: related_to
---

# Effective Potential

The **Effective Potential** ($V(r)$) simplifies complex two-dimensional orbital problems into a one-dimensional visualization, treating a particle like a marble rolling in a track.

It groups the kinetic energy associated with angular motion (the "centrifugal" potential, $U_c = \frac{l^2}{2\mu r^2}$) together with the actual physical potential energy $U(r)$:

$$V(r) \equiv U(r) + \frac{l^2}{2\mu r^2}$$

## Analysis of Orbits
The total energy $E$ of the particle against the $V(r)$ curve determines its trajectory:
- **Unbounded ($E \ge 0$)**: The particle comes from infinity, hits the centrifugal wall (periapsis), and escapes back to infinity (e.g., hyperbolic trajectory).
- **Bounded ($V_{min} < E < 0$)**: Trapped in the "valley" between two turning points ($r_{min}$ and $r_{max}$). Oscillations trace an elliptical orbit.
- **Circular ($E = V_{min}$)**: The particle sits at the exact bottom of the potential well. The radius is locked at one distance with no radial kinetic energy.
