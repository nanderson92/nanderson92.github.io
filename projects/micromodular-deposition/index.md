---
layout: page
title: Micromodular Printed Electronics Deposition
category: Flagship Case Study
subtitle: Substrate-mediated droplet deposition, device placement, and process-window development for scalable printed electronics.
---

## Summary

I am investigating how substrate boundary conditions control droplet deposition, microscale device placement, and process reproducibility in micromodular printed electronics.

<div class="buildout-note">Case study buildout in progress — current focus: method, metrics, and representative figures. Recreated schematics are used where raw lab visuals are not appropriate for public sharing.</div>

<div class="role-block">
  <p class="system-label small">MY ROLE</p>
  <p>
    Designed experiments, captured top/side-view droplet videos, extracted contact-line dynamics, compared substrate boundary conditions, and developed process-window metrics for repeatable deposition.
  </p>
</div>

## Problem / motivation

Printed electronics could enable more distributed and flexible manufacturing of electronic systems. A key challenge is not only fabricating devices, but assembling them reproducibly. When a suspension droplet dries, suspended microdevices can accumulate nonuniformly, often forming edge-heavy deposits that reduce placement fidelity and complicate later interconnect printing.

## Preliminary observation and visual artifact

<div class="result-callout">
  <p class="system-label small">PRELIMINARY OBSERVATION</p>
  <p>
    Early deposition trials suggest that porous substrate boundary conditions change the droplet footprint and can reduce edge-dominated accumulation compared with a nonporous glass control. The current analysis workflow is focused on converting these observations into repeatable metrics: r(t), θ(t), V(t), edge/center ratio, and areal-density uniformity.
  </p>
</div>

<figure class="technical-figure">
  <img src="{{ '/assets/images/deposition-pattern-schematic.svg' | relative_url }}" alt="Recreated schematic comparing edge-heavy glass deposition with more distributed porous-substrate deposition">
  <figcaption>Recreated schematic based on pilot observations. This is not raw microscopy data; it is a public-safe visual summary of the deposition-pattern comparison being quantified.</figcaption>
</figure>

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

The central engineering question is:

> What substrate boundary conditions produce repeatable, spatially uniform deposition of micromodular electronic devices?

The project treats the substrate as an active boundary condition rather than a passive surface. Wetting, imbibition, evaporation, and contact-line behavior all influence where devices end up after deposition.

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

<figure class="technical-figure compact-figure">
  <img src="{{ '/assets/images/droplet-metric-panel.svg' | relative_url }}" alt="Representative metric extraction panel for droplet radius, contact angle, and volume over time">
  <figcaption>Representative metric panel showing the analysis targets from droplet videos. Replace with measured traces once the public data export is ready.</figcaption>
</figure>

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

The goal is to connect observed droplet behavior to process descriptors. Instead of treating deposition quality as purely empirical, the project frames it as a coupled transport/process-window problem involving evaporation, imbibition, pinning, and device crowding.

## Manufacturing relevance

A manufacturable printed-electronics assembly process needs repeatable placement, compatible substrate boundary conditions, and predictable integration with later interconnect printing. This project aims to define measurable descriptors that make deposition conditions easier to compare, tune, and eventually scale.

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
    <h3>Design rule</h3>
    <p>Translate metrics into substrate-selection logic and process constraints for scalable assembly.</p>
  </div>
</div>
