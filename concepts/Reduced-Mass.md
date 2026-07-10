---
title: Reduced Mass
category: concept
tags: [mechanics, simplification]
sources: ["textbook/8.md"]
created: 2026-07-09T02:37:00
updated: 2026-07-09T02:37:00
base_confidence: 0.5
lifecycle: draft
tier: supporting
summary: A mathematical technique used to simplify the analysis of a two-body system by mapping it onto an equivalent one-body problem.
provenance: {extracted: 1.0, inferred: 0.0, ambiguous: 0.0}
relationships:
  - target: "[[concepts/Central-Force-Motion]]"
    type: related_to
---

# Reduced Mass

**Reduced mass** ($\mu$) is a foundational technique in classical mechanics used to simplify the analysis of a two-body system interacting via a central force.

Instead of tracking 6 degrees of freedom for two bodies in a 3D space, the system is analyzed relative to the center of mass. This allows the two-body problem to be mathematically mapped onto an equivalent one-body problem, consisting of a single, imaginary particle of mass $\mu$ orbiting a fixed origin at a relative distance $r$.

$$\mu \equiv \frac{m_{1}m_{2}}{m_{1}+m_{2}}$$

## Key Takeaways
- $\mu$ is always strictly less than the mass of the lighter particle.
- If $m_{1} \gg m_{2}$, then $\mu \approx m_{2}$. The system behaves almost exactly as if the larger mass is totally stationary.
- If $m_{1} = m_{2}$, then $\mu = m/2$. Both bodies orbit a shared empty point in space midway between them.
