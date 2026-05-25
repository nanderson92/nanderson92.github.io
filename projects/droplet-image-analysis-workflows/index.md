---
layout: page
title: Droplet and Image Analysis Workflows
category: Computation / Experimental Measurement
subtitle: Image segmentation, calibration, droplet tracking, and time-series extraction for process metrics.
---

## Summary

This case file covers workflows for converting microscopy videos and droplet images into quantitative measurements that support process engineering decisions.

## Problem / motivation

Raw microscopy videos are not engineering metrics by themselves. To compare substrates, droplets, and process conditions, the images must be segmented, calibrated, checked, and converted into time-series outputs such as droplet radius, contact angle, volume, or deposition distribution.

## System schematic

<div class="project-schematic schematic-compute" aria-label="Representative image analysis workflow schematic">
  <div class="compute-flow"><span>VIDEO</span><i></i><span>SEGMENT</span><i></i><span>CALIBRATE</span><i></i><span>METRICS</span></div>
  <p>Representative public workflow for converting raw video into comparable process variables.</p>
</div>

## My role

<div class="role-block">
  <p>Built and troubleshot image-analysis workflows, calibrated videos, extracted droplet boundaries and time-series variables, and connected raw visual observations to process metrics.</p>
</div>

## Technical challenge

The core challenge is repeatability. Edge detection, contrast, scale calibration, thresholding, and frame handling can change the extracted metric. A useful workflow must be consistent enough to compare conditions and transparent enough to audit.

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

## Engineering interpretation

The value of this project is measurement discipline. A better image workflow makes experimental comparisons stronger because it turns visual behavior into traceable variables that can be linked to substrate and process conditions.

<div class="case-cta-row">
 <a class="button primary" href="{{ '/projects/' | relative_url }}">View all case files</a>
 <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Download Resume</a>
 <a class="button tertiary" href="mailto:{{ site.email }}">Contact</a>
</div>
