---
layout: page
title: Micromodular Electronics Deposition
category: Flagship Case Study
tags: Semiconductors · Process Development · Interfacial Transport · Automation & Data
subtitle: Substrate-controlled process windows for stochastic microdevice placement in micromodular printed electronics.
---

## Summary

This project investigates how substrate boundary conditions control droplet deposition, microscale device placement, and process reproducibility in micromodular printed electronics. The larger manufacturing vision is simple but difficult: suspend modular electronic devices in a liquid ink, deposit them where they are useful, then interconnect them into circuits.

<div class="buildout-note">Case study buildout in progress — public-safe schematics are used where raw lab visuals are not appropriate for public sharing.</div>

<div class="role-block">
  <p class="system-label small">MY ROLE</p>
  <p>Designed substrate/backing experiments, captured top- and side-view droplet videos, extracted contact-line dynamics, compared deposition behavior across boundary conditions, and built Python/ImageJ workflows for turning videos into process metrics.</p>
</div>

## Problem / motivation

Printed electronics is not only a materials problem; it is an assembly problem. When a droplet containing microdevices dries or imbibes into a substrate, devices can raft, crowd, pin near the contact line, and accumulate nonuniformly. That nonuniformity reduces placement fidelity and makes downstream interconnect printing harder.

The practical question is:

> What substrate boundary conditions produce repeatable, spatially useful deposition instead of edge-heavy accumulation?


## Where this project fits in the workflow

<figure class="wide-figure">
  <img src="{{ '/assets/images/micromodular-workflow-deposition-focus.png' | relative_url }}" alt="High-level micromodular electronics workflow with the deposition subsystem highlighted across suspending components in ink and printing components." loading="lazy">
  <figcaption><strong>Micromodular electronics workflow.</strong> The rounded rectangle highlights the deposition subsystem: suspending fabricated components in ink and printing them onto the substrate in a way that produces useful placement for downstream circuit assembly.</figcaption>
</figure>

## Public-safe system schematic

<div class="project-schematic" aria-label="Representative schematic of droplet, substrate, and suspended microdevices">
  <div class="droplet-system">
    <div class="droplet"></div>
    <div class="devices"></div>
    <div class="substrate"></div>
    <span class="callout-label one">suspension droplet</span>
    <span class="callout-label two">porous / coated process boundary</span>
  </div>
</div>

## Engineering framing

<div class="matrix">
  <div class="matrix-card"><h3>Process input</h3><p>Droplet volume, solvent, particle/device loading, substrate, backing layer, and deposition method.</p></div>
  <div class="matrix-card"><h3>Transport behavior</h3><p>Spreading, imbibition, evaporation, contact-line pinning, edgeward flow, and device crowding.</p></div>
  <div class="matrix-card"><h3>Manufacturing output</h3><p>Areal density, edge/center ratio, placement fidelity, repeatability, and downstream interconnect feasibility.</p></div>
</div>

## Variables studied

| Variable | Why it matters |
|---|---|
| Substrate porosity / permeability | Controls liquid uptake and vertical drain rate. |
| Backing condition | Changes whether the porous substrate behaves like a drain, membrane, or supported surface. |
| Contact angle / wetting | Sets footprint size, spreading dynamics, and transport length scale. |
| Contact-line pinning | Influences coffee-ring-like accumulation and edge crowding. |
| Evaporation vs. imbibition | Determines whether flow is dominated by drying or liquid uptake. |
| Device loading | Affects crowding, raft interactions, and useful areal density. |

## Methods and tools

<div class="two-col">
  <div class="matrix-card">
    <h3>Experimental methods</h3>
    <p>Sessile droplet deposition, AAO/substrate comparisons, backing-layer studies, optical microscopy, top-view videos, side-view videos, and process observation.</p>
  </div>
  <div class="matrix-card">
    <h3>Analysis methods</h3>
    <p>Droplet-radius extraction, contact-line tracking, deposition-pattern quantification, radial density maps, edge/center ratio, process-window framing, and statistical comparison.</p>
  </div>
</div>

<div class="badge-row">
  <span class="badge">Keyence</span>
  <span class="badge">Rame-Hart</span>
  <span class="badge">Python</span>
  <span class="badge">ImageJ/Fiji</span>
  <span class="badge">JMP</span>
  <span class="badge">Optical Microscopy</span>
</div>

## Embedded technical artifact: droplet and device tracking workflow

The previous standalone “Droplet and Image Analysis Workflows” page is now folded into this project because the code/workflow exists to solve the deposition problem.

<div class="matrix">
  <div class="matrix-card"><h3>Inputs</h3><p>Microscopy videos, still frames, scale calibration images, substrate labels, and frame-rate metadata.</p></div>
  <div class="matrix-card"><h3>Processing</h3><p>Frame extraction, crop/rotation handling, segmentation, threshold checks, edge tracking, and validation against raw video.</p></div>
  <div class="matrix-card"><h3>Outputs</h3><p>r(t), θ(t), V(t) proxies, radial deposition maps, edge/center ratio, areal density, and comparison plots.</p></div>
</div>

## Current / planned portfolio artifacts

<div class="metric-grid">
  <div class="metric-card"><h3>r(t)</h3><div class="plot-placeholder" aria-hidden="true"></div></div>
  <div class="metric-card"><h3>Edge / center ratio</h3><div class="plot-placeholder" aria-hidden="true"></div></div>
  <div class="metric-card"><h3>Process window</h3><div class="plot-placeholder" aria-hidden="true"></div></div>
</div>

## Engineering interpretation

The goal is to turn qualitative droplet observations into process descriptors. Instead of saying one substrate “looks better,” the project asks which boundary conditions create measurable improvements in deposition uniformity, useful center density, and repeatability.

## Manufacturing relevance

A scalable printed-electronics assembly process needs repeatable placement, measurement discipline, and process windows that can survive material and substrate variation. This project connects chemical-engineering transport thinking to a semiconductor-manufacturing assembly bottleneck.

## Next steps

<div class="matrix">
  <div class="matrix-card"><h3>Add public-safe figures</h3><p>Recreated droplet/deposition graphics, one annotated frame, and one clean comparison plot.</p></div>
  <div class="matrix-card"><h3>Lock metrics</h3><p>Define edge/center ratio, useful areal density, and acceptable repeatability thresholds.</p></div>
  <div class="matrix-card"><h3>Build story</h3><p>Connect AAO-like behavior to a substrate-agnostic coating or boundary-condition design rule.</p></div>
</div>
