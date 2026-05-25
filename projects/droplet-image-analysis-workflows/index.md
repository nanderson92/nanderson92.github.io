---
layout: page
title: Droplet and Image Analysis Workflows
category: Video → metric pipeline
subtitle: Image segmentation, calibration, droplet tracking, and time-series extraction for process metrics.
---

## Summary

Raw microscopy videos are not engineering metrics by themselves. I built workflows that turn video into comparable variables: droplet radius, contact-line motion, contact angle, volume proxy, and deposition distribution.

## Problem / motivation

To compare substrates, droplets, and process conditions, images have to be segmented, calibrated, checked, and converted into time-series outputs. The hard part was making the workflow repeatable enough that the metric reflected the experiment rather than a thresholding artifact.

## System schematic

<div class="process-map compact-flow-map" aria-label="Representative image analysis workflow schematic">
 <div class="process-map-stage"><p>VIDEO</p><span>raw frames</span><span>scale bar</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage"><p>SEGMENT</p><span>edge detection</span><span>threshold checks</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage"><p>CALIBRATE</p><span>pixels to length</span><span>time base</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage decision-stage"><p>METRICS</p><span>r(t), θ(t), V(t), edge/center ratio</span></div>
</div>

## My role

<div class="role-block">
  <p>Built and troubleshot image-analysis workflows, calibrated videos, extracted droplet boundaries and time-series variables, and connected raw visual observations to process metrics.</p>
</div>

## Variables extracted

| Metric | Why it matters |
|---|---|
| r(t) | Tracks droplet footprint and spreading/imbibition behavior. |
| θ(t) | Connects wetting and contact-line dynamics to substrate behavior. |
| V(t) | Helps separate evaporation from liquid uptake or drainage. |
| Edge/center ratio | Quantifies coffee-ring-like deposition bias. |
| Areal density | Measures how many devices occupy useful regions of the substrate. |

## Public artifact set

<div class="matrix">
  <div class="matrix-card"><h3>Annotated frame format</h3><p>Public-safe image layout showing droplet edge, scale, and region of interest.</p></div>
  <div class="matrix-card"><h3>Metric plots</h3><p>r(t), θ(t), V(t), and deposition-distribution plots as the core measurement outputs.</p></div>
  <div class="matrix-card"><h3>Workflow checklist</h3><p>Repeatable procedure for converting raw videos into comparable metrics.</p></div>
</div>

## Methods and tools

<div class="two-col">
  <div class="matrix-card"><h3>Image workflow</h3><p>Frame extraction, crop/scale handling, segmentation, threshold checks, edge tracking, and validation against raw video.</p></div>
  <div class="matrix-card"><h3>Analysis workflow</h3><p>Time normalization, plotting, radial distributions, outlier checks, and process-condition comparisons.</p></div>
</div>

<div class="badge-row"><span class="badge">Python</span><span class="badge">ImageJ/Fiji</span><span class="badge">MATLAB</span><span class="badge">Segmentation</span><span class="badge">Time Series</span></div>

## What I’d do next

The next version would turn the workflow into a small reproducible tool: load video, confirm calibration, extract contact line, export a standard plot, and save every processing choice. That audit trail matters because small segmentation choices can change the process conclusion.

<div class="case-cta-row">
 <a class="button primary" href="{{ '/projects/' | relative_url }}">View all projects</a>
 <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Download Resume</a>
 <a class="button tertiary" href="mailto:{{ site.email }}">Contact</a>
</div>
