---
layout: page
title: Printed Interconnect Reliability Analysis
category: Reliability / Experimental Analysis Case Study
subtitle: Resistance drift, environmental stress response, and data interpretation for printed interconnects.
---

## Summary

This project area evaluates how printed conductive features change under time, humidity, temperature, or handling-related stress.

<div class="buildout-note">Case study buildout in progress — current focus: method, metrics, and representative figures. This page is structured to make the project usable before the final data package is added.</div>

<div class="role-block">
  <p class="system-label small">MY ROLE</p>
  <p>Organized resistance measurements, compared aging/stress behavior, and framed results around reliability drift, failure intervals, and process implications.</p>
</div>

## Problem / motivation

Electrical resistance can drift for reasons that are physical, process-related, or measurement-related. The analysis challenge is to distinguish meaningful degradation from noise and translate it into a reliability decision.

## System

<div class="technical-system-card">
  <p class="system-label small">SYSTEM</p>
  <h3>Printed Ag interconnect + environmental stress + resistance measurement + statistical comparison</h3>
</div>

## Variables / decisions

| Variable or decision | Why it matters |
|---|---|
| Stress condition | Temperature, humidity, duration, and handling can accelerate different failure modes. |
| Initial resistance | Baseline variation affects interpretation of percent change and drift. |
| Measurement cadence | Determines whether transient behavior or late-stage failure is visible. |
| Failure definition | Controls how reliability outcomes are counted and compared. |

## Methods and tools

<div class="two-col">
  <div class="matrix-card"><h3>Resistance tracking</h3><p>Collect time-series or before/after measurements to observe drift and failure behavior.</p></div><div class="matrix-card"><h3>Statistical interpretation</h3><p>Use comparison plots, distribution checks, and JMP workflows to identify meaningful shifts.</p></div>
</div>

<div class="badge-row">
  <span class="badge">JMP</span>
<span class="badge">Excel</span>
<span class="badge">Python</span>
<span class="badge">4-Point Probe</span>
<span class="badge">Reliability</span>
<span class="badge">ANOVA</span>
</div>

## Outputs / metrics

<div class="matrix">
  <div class="matrix-card"><h3>Reliability curve</h3><p>Resistance versus time or stress exposure.</p></div><div class="matrix-card"><h3>Drift metric</h3><p>Normalized change, failure interval, or pass/fail summary.</p></div><div class="matrix-card"><h3>Process implication</h3><p>Interpretation for fabrication, storage, or handling conditions.</p></div>
</div>

## Engineering interpretation

The project converts raw resistance measurements into reliability-relevant outputs: drift, spread, outliers, possible failure thresholds, and process-level recommendations.

## Manufacturing relevance

Printed electronics manufacturing depends on conductive features that remain stable enough for routing and device integration. Reliability analysis connects lab fabrication to production viability.

## Next steps

<div class="matrix">
  <div class="matrix-card"><h3>Buildout</h3><p>Add representative figures, assumptions, sample calculations, and final artifact screenshots.</p></div>
  <div class="matrix-card"><h3>Validation</h3><p>Clarify checks, constraints, and uncertainty before presenting final conclusions.</p></div>
  <div class="matrix-card"><h3>Portfolio output</h3><p>Convert the project into a concise engineering case file for recruiters and technical managers.</p></div>
</div>
