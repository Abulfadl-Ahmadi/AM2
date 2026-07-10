---
title: Central-Force Motion
category: concept
tags: [mechanics, orbital-dynamics]
sources: ["textbook/8.md"]
created: 2026-07-09T02:37:00
updated: 2026-07-09T02:37:00
base_confidence: 0.5
lifecycle: draft
tier: core
summary: A central force is one that always points directly toward or away from a fixed point and whose magnitude depends only on the distance from that point.
provenance: {extracted: 1.0, inferred: 0.0, ambiguous: 0.0}
relationships:
  - target: "[[concepts/Reduced-Mass]]"
    type: related_to
  - target: "[[concepts/Effective-Potential]]"
    type: related_to
---

# Central-Force Motion

A **central force** in classical mechanics is an interaction where the force vector acting on a particle always points directly toward or away from a fixed point (typically the origin or the center of another body). The magnitude of this force depends exclusively on the distance $r$ between the interacting bodies.

## Key Properties
- **Spherical Symmetry**: The physical setup looks exactly the same regardless of coordinate axis rotation, leading to the conservation of angular momentum ($L$).
- **Planar Motion**: Because $L = r \times p$ is conserved, both the position vector $r$ and momentum vector $p$ always remain perpendicular to $L$, physically confining the particle's entire orbit to a single flat 2D plane.
- **Kepler's Second Law**: A line drawn from the central body to the orbiting particle sweeps out equal areas in equal amounts of time. This is true for *all* central-force motion, not just inverse-square laws.

## Importance
Central-force motion describes fundamental interactions across vastly different scales, from the macroscopic (Newton's Law of Universal Gravitation) to the microscopic (Coulomb's Law of Electrostatics). It remains one of the few complex physical problems in mechanics that yields a complete, exact, analytical solution.
