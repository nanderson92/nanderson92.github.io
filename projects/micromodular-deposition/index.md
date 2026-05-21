---
layout: page
title: Micromodular Printed Electronics Deposition
category: Flagship Case Study
subtitle: Recreated/schematic visuals for substrate-mediated droplet deposition, process-window metrics, and manufacturable printed electronics assembly.
---

<div class="role-block">
  <p class="system-label small">SUMMARY</p>
  <p>
    This in-progress research case study investigates how porous substrate boundary conditions control droplet behavior, microscale device placement, and deposition uniformity in micromodular printed electronics.
  </p>
</div>

## Problem / motivation

Printed electronics could enable lower-cost, distributed, and flexible manufacturing of electronic systems. A core challenge is not only fabricating devices, but assembling them reproducibly into useful circuits. In suspension-based deposition, drying and imbibing droplets can produce nonuniform device distributions, edge-heavy deposits, and placement challenges for later interconnect printing.

## System schematic

<div class="project-schematic" aria-label="Recreated schematic of droplet, substrate, and suspended microdevices">
  <div class="droplet-system">
    <div class="droplet"></div>
    <div class="devices"></div>
    <div class="substrate"></div>
    <span class="callout-label one">IPA droplet + devices</span>
    <span class="callout-label two">Porous substrate boundary condition</span>
  </div>
</div>

<p class="caption">Representative recreated schematic. This is not a lab-confidential image or measured dataset.</p>

## My role

<div class="role-block">
  <p>
    Designed experiments, captured top/side-view droplet videos, extracted contact-line dynamics, compared substrate boundary conditions, and developed process-window metrics for manufacturable deposition.
  </p>
</div>

## Technical challenge

<div class="translation-strip">
  <div>
    <h3>Research Signal</h3>
    <p>Droplet spreading, drying, imbibition, pinning, visible deposition patterns, and device motion.</p>
  </div>
  <div>
    <h3>Engineering Metric</h3>
    <p>r(t), θ(t), V(t), edge/center ratio, areal density, and deposition uniformity descriptors.</p>
  </div>
  <div>
    <h3>Manufacturing Rule</h3>
    <p>Substrate selection logic, process-window boundaries, and routing-compatible deposition conditions.</p>
  </div>
</div>

## Variables studied

<table>
  <thead>
    <tr><th>Variable</th><th>Why it matters</th><th>Engineering relevance</th></tr>
  </thead>
  <tbody>
    <tr><td>Substrate porosity</td><td>Controls drainage and imbibition.</td><td>Changes how fast solvent leaves the droplet.</td></tr>
    <tr><td>Contact angle</td><td>Affects spreading and footprint.</td><td>Influences final deposit area and routing compatibility.</td></tr>
    <tr><td>Pinning behavior</td><td>Controls contact-line motion.</td><td>Can intensify or suppress edge-heavy deposition.</td></tr>
    <tr><td>Evaporation / imbibition balance</td><td>Sets timescales for transport.</td><td>Defines candidate process windows.</td></tr>
    <tr><td>Device concentration</td><td>Controls crowding and statistics.</td><td>Impacts placement uniformity and yield logic.</td></tr>
  </tbody>
</table>

## Methods and tools

<div class="badge-row method-stack">
  <span class="badge">Optical microscopy</span>
  <span class="badge">Top/side-view video</span>
  <span class="badge">Droplet tracking</span>
  <span class="badge">Contact-line dynamics</span>
  <span class="badge">Python</span>
  <span class="badge">ImageJ/Fiji</span>
  <span class="badge">JMP</span>
</div>

## Data / metrics to extract

<div class="metric-grid">
  <div class="metric-card">
    <h3>r(t)</h3>
    <div class="plot-placeholder"></div>
  </div>
  <div class="metric-card">
    <h3>θ(t)</h3>
    <div class="plot-placeholder alt"></div>
  </div>
  <div class="metric-card">
    <h3>V(t)</h3>
    <div class="plot-placeholder third"></div>
  </div>
</div>

<div class="artifact-grid page-artifacts">
  <div class="artifact-card artifact-droplet"><span>Deposition uniformity diagram</span></div>
  <div class="artifact-card artifact-window"><span>Process-window map placeholder</span></div>
  <div class="artifact-card artifact-compute"><span>Variable extraction panel</span></div>
  <div class="artifact-card artifact-process"><span>Experiment-to-metric flow</span></div>
</div>

<p class="caption">Plots and panels are placeholders for recreated/abstracted metrics until finalized data is ready for public release.</p>

## Engineering interpretation

The project frames substrate behavior as a process-defining boundary condition. The goal is to connect wetting, imbibition, pinning, and droplet drying behavior to measurable descriptors that predict whether microscale devices deposit uniformly enough for downstream circuit assembly.

## Manufacturing relevance

A useful deposition process must be repeatable, measurable, and compatible with later manufacturing steps. This case study is structured around that translation: from raw video and substrate observations to process windows, substrate-selection logic, and manufacturable deposition metrics.

## Next steps

<div class="matrix">
  <div class="matrix-card">
    <h3>Quantify</h3>
    <p>Extract radius, contact angle, volume, deposition uniformity, and edge/center ratios across conditions.</p>
  </div>
  <div class="matrix-card">
    <h3>Compare</h3>
    <p>Compare substrate boundary conditions and backing configurations using consistent metrics.</p>
  </div>
  <div class="matrix-card">
    <h3>Translate</h3>
    <p>Convert trends into process-window maps and substrate-selection rules.</p>
  </div>
</div>
