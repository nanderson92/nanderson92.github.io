---
layout: page
title: Printed Interconnect Reliability Analysis
category: Reliability / Experimental Analysis
subtitle: Resistance drift, environmental stress response, and manufacturing-relevant reliability interpretation.
---
## Summary

This case study focuses on how printed interconnects change under aging or environmental stress, with emphasis on converting resistance measurements into reliability interpretation.

<div class="buildout-note">Case study buildout in progress — current focus: method, metrics, and representative figures.</div>

## Problem / motivation

Printed electronics depend on conductive interconnects that remain stable across handling, humidity, temperature, and time. Resistance drift can indicate material instability, process variation, poor curing/sintering, or early reliability failure.

## System schematic

<div class="project-schematic schematic-reliability" aria-label="Representative resistance drift schematic">
  <div class="signal-line"></div>
  <p>Representative reliability-curve motif · replace with public-safe experimental plot when ready.</p>
</div>

## My role

<div class="role-block">
  <p>Organized resistance data, compared stressed and baseline conditions, used statistical analysis to detect changes, and framed reliability behavior in terms of process stability and manufacturing risk.</p>
</div>

## Technical challenge

The engineering challenge is distinguishing measurement noise from meaningful drift. A useful reliability analysis needs consistent measurement protocol, clear stress conditions, time-based comparison, and interpretation that ties data back to process decisions.

## Variables studied

| Variable | Why it matters |
|---|---|
| Initial resistance | Baseline for drift and device-to-device variation. |
| Time under stress | Reveals gradual degradation or stabilization behavior. |
| Temperature / humidity exposure | Accelerates failure mechanisms and process weaknesses. |
| Interconnect geometry | Affects current path, resistance, and failure sensitivity. |
| Processing history | Cure/sintering and handling can strongly affect conductivity. |

## Methods and tools

<div class="two-col">
  <div class="matrix-card"><h3>Experimental analysis</h3><p>Resistance tracking, stress-condition comparison, failure interval framing, drift interpretation, and measurement checks.</p></div>
  <div class="matrix-card"><h3>Statistics / visualization</h3><p>JMP comparisons, trend plots, summary tables, and exploratory reliability figures.</p></div>
</div>

<div class="badge-row"><span class="badge">JMP</span><span class="badge">Excel</span><span class="badge">Python</span><span class="badge">Reliability</span><span class="badge">Resistance Data</span></div>

## Outputs to add

<div class="matrix">
  <div class="matrix-card"><h3>Resistance vs. time</h3><p>Plot showing drift, stabilization, or failure behavior.</p></div>
  <div class="matrix-card"><h3>Stress comparison table</h3><p>Baseline vs. stressed conditions with summary statistics.</p></div>
  <div class="matrix-card"><h3>Manufacturing implication</h3><p>Short statement connecting drift to process control or reliability risk.</p></div>
</div>

## Engineering interpretation

The value of this project is not just plotting resistance. It is turning electrical measurements into a practical decision: whether the interconnect process appears stable enough for downstream integration or needs additional process control.

## Next steps

Add a public-safe resistance plot, include statistical comparisons, and define a failure/drift threshold that can support a manufacturing decision.
