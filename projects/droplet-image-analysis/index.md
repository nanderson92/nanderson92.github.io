---
layout: page
title: Droplet and Image Analysis Workflows
category: Computation / Image Analysis Case Study
subtitle: Image-processing workflows for turning droplet videos and microscopy frames into engineering metrics.
---

## Summary

This project area focuses on extracting usable measurements from experimental images: droplet radius, contact angle, volume proxies, deposit distributions, and time-normalized trends.

<div class="buildout-note">Case study buildout in progress — current focus: method, metrics, and representative figures. This page is structured to make the project usable before the final data package is added.</div>

<div class="role-block">
  <p class="system-label small">MY ROLE</p>
  <p>Designed image-analysis workflows, handled calibration and segmentation issues, and mapped raw video observations into metrics that can support process comparisons.</p>
</div>

## Problem / motivation

Experimental videos are visually useful but not yet engineering evidence. The challenge is to create repeatable measurement workflows that can survive noise, contrast changes, and frame-to-frame variation.

## System

<div class="technical-system-card">
  <p class="system-label small">SYSTEM</p>
  <h3>Microscopy video + scale calibration + segmentation + time-series extraction + validation checks</h3>
</div>

## Variables / decisions

| Variable or decision | Why it matters |
|---|---|
| Pixel-to-length calibration | Converts visual measurements into physical distances. |
| Segmentation threshold | Controls droplet edge and deposit detection. |
| Frame rate | Determines time resolution for r(t), θ(t), and volume trends. |
| Validation check | Prevents image-processing artifacts from becoming false conclusions. |

## Methods and tools

<div class="two-col">
  <div class="matrix-card"><h3>Image preprocessing</h3><p>Crop, rotate, scale, and prepare image stacks for measurement.</p></div><div class="matrix-card"><h3>Metric extraction</h3><p>Track droplet radius, contact-line motion, area, and distribution descriptors over time.</p></div>
</div>

<div class="badge-row">
  <span class="badge">Python</span>
<span class="badge">ImageJ/Fiji</span>
<span class="badge">MATLAB</span>
<span class="badge">Microscopy</span>
<span class="badge">Segmentation</span>
<span class="badge">Calibration</span>
</div>

## Outputs / metrics

<div class="matrix">
  <div class="matrix-card"><h3>r(t), θ(t), V(t)</h3><p>Time-series variables for droplet behavior.</p></div><div class="matrix-card"><h3>Deposit map</h3><p>Spatial distribution of microdevices or proxy particles.</p></div><div class="matrix-card"><h3>Workflow note</h3><p>Documented steps that make analysis repeatable across conditions.</p></div>
</div>

## Engineering interpretation

The project makes experimental observation quantitative. The intended output is a workflow that can compare substrates and conditions with the same measurement logic.

## Manufacturing relevance

Manufacturing decisions require repeatable measurements. Image-analysis workflows help turn visual lab behavior into metrics suitable for screening, optimization, and scale-up discussions.

## Next steps

<div class="matrix">
  <div class="matrix-card"><h3>Buildout</h3><p>Add representative figures, assumptions, sample calculations, and final artifact screenshots.</p></div>
  <div class="matrix-card"><h3>Validation</h3><p>Clarify checks, constraints, and uncertainty before presenting final conclusions.</p></div>
  <div class="matrix-card"><h3>Portfolio output</h3><p>Convert the project into a concise engineering case file for recruiters and technical managers.</p></div>
</div>
