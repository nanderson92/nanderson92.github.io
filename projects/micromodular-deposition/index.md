---
layout: page
title: Micromodular Printed Electronics Deposition
category: Flagship Case Study
subtitle: Substrate-mediated droplet deposition, microscale device placement, and process-window development for scalable printed electronics.
---

## Summary

I am investigating how substrate boundary conditions control droplet deposition, microscale device placement, and process reproducibility in micromodular printed electronics.

<div class="role-block">
  <p class="label small">MY ROLE</p>
  <p>
    Designed experiments, captured top/side-view droplet videos, extracted contact-line dynamics, compared substrate boundary conditions, and developed process-window metrics for manufacturable deposition.
  </p>
</div>

## Problem / motivation

Printed electronics could enable more distributed and flexible manufacturing of electronic systems. A key challenge is not only fabricating devices, but assembling them reproducibly. When a suspension droplet dries, suspended microdevices can accumulate nonuniformly, often forming edge-heavy deposits that reduce placement fidelity and complicate later interconnect printing.

## System schematic

<div class="project-schematic" aria-label="Representative schematic of droplet, substrate, and suspended microdevices">
  <div class="droplet-system">
    <div class="droplet"></div>
    <div class="devices"></div>
    <div class="substrate"></div>
    <span class="callout-label one">recreated schematic · not raw data</span>
    <span class="callout-label two">porous substrate boundary condition</span>
  </div>
</div>

## Technical challenge

The core engineering question is:

> What substrate boundary conditions produce repeatable, spatially uniform, and manufacturable deposition of micromodular electronic devices?

The substrate is treated as an active process boundary condition rather than a passive surface. Wetting, imbibition, evaporation, and contact-line behavior all influence where devices end up after deposition.

## Variables studied

| Variable | Why it matters |
|---|---|
| Substrate porosity | Controls liquid drainage and imbibition. |
| Contact angle | Affects spreading, droplet footprint, and device transport length scale. |
| Pinning behavior | Influences edge accumulation and coffee-ring-like deposition. |
| Evaporation rate | Controls concentration and transport timescale. |
| Device density | Affects crowding, interactions, and placement statistics. |
| Droplet volume | Changes drying time, footprint, and process repeatability. |

## Methods and tools

<div class="two-col">
  <div class="matrix-card">
    <h3>Experimental methods</h3>
    <p>Sessile droplet deposition, substrate comparison, optical microscopy, top-view videos, side-view videos, and process observation.</p>
  </div>
  <div class="matrix-card">
    <h3>Analysis methods</h3>
    <p>Contact-line tracking, droplet-radius extraction, deposition-pattern quantification, process-window framing, and statistical comparison.</p>
  </div>
</div>

<div class="badge-row">
  <span class="badge">Keyence</span>
  <span class="badge">Python</span>
  <span class="badge">ImageJ/Fiji</span>
  <span class="badge">JMP</span>
  <span class="badge">Optical Microscopy</span>
  <span class="badge">Droplet Tracking</span>
</div>

## Data / metrics to extract

<div class="metric-grid">
  <div class="metric-card">
    <h3>r(t)</h3>
    <div class="plot-placeholder" aria-hidden="true"></div>
  </div>
  <div class="metric-card">
    <h3>θ(t)</h3>
    <div class="plot-placeholder" aria-hidden="true"></div>
  </div>
  <div class="metric-card">
    <h3>V(t)</h3>
    <div class="plot-placeholder" aria-hidden="true"></div>
  </div>
</div>

Potential engineering metrics include:

- Areal density uniformity
- Edge-to-center deposition ratio
- Droplet radius versus time
- Contact angle versus time
- Droplet volume versus time
- Imbibition/evaporation flow comparison
- Placement fidelity metrics
- Process maps for substrate selection

## Engineering interpretation

The goal is to connect observed droplet behavior to process descriptors. Instead of treating deposition quality as purely empirical, the project frames it as a coupled transport problem involving evaporation, imbibition, pinning, and device crowding.

## Manufacturing relevance

A manufacturable printed-electronics assembly process needs repeatable placement, compatible substrate boundary conditions, and predictable integration with later interconnect printing. This project aims to define measurable descriptors that make deposition conditions easier to compare, tune, and scale.

## Next steps

<div class="matrix">
  <div class="matrix-card">
    <h3>Data extraction</h3>
    <p>Convert top/side-view videos into consistent r(t), θ(t), V(t), and deposition-distribution measurements.</p>
  </div>
  <div class="matrix-card">
    <h3>Process windows</h3>
    <p>Compare substrates and backing conditions using normalized metrics and repeatability checks.</p>
  </div>
  <div class="matrix-card">
    <h3>Decision logic</h3>
    <p>Translate metrics into substrate-selection logic and process constraints for scalable assembly.</p>
  </div>
</div>
