---
title: Hohmann Transfer
category: concept
tags: [mechanics, orbital-dynamics, space-navigation]
sources: ["textbook/8.md"]
created: 2026-07-09T02:37:00
updated: 2026-07-09T02:37:00
base_confidence: 0.5
lifecycle: draft
tier: core
summary: The most economical method of interplanetary transfer involving two engine burns to move between coplanar circular orbits.
provenance: {extracted: 1.0, inferred: 0.0, ambiguous: 0.0}
relationships:
  - target: "[[concepts/Central-Force-Motion]]"
    type: related_to
  - target: "[[concepts/Gravity-Assist]]"
    type: related_to
---

# Hohmann Transfer

A **Hohmann Transfer** is a highly energy-efficient orbital maneuver used to move a spacecraft between two circular, coplanar orbits. Since fuel is heavy and expensive to launch, this transfer minimizes the required $\Delta v$ (total velocity change).

## Mechanics
It involves two precisely timed engine burns:
1. **First Burn (Departure)**: Fired parallel to the spacecraft's motion (prograde) to add kinetic energy, stretching the initial circular orbit into an elliptical transfer orbit. The apoapsis (highest point) of this new ellipse intersects the destination orbit.
2. **Second Burn (Arrival)**: Fired at the apoapsis of the transfer orbit to circularize the trajectory and match the orbital speed of the destination body.

## Limitations
While energy-efficient, Hohmann transfers are extremely slow. For example, a round trip to Mars requires roughly 2.7 years due to the necessary wait time for correct planetary alignment before the return trip.
