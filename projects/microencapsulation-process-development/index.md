---
layout: page
title: Stem-Cell Microencapsulation
category: 20× throughput increase
date_range: Summer 2025
affiliation: Mayo Clinic · Rochester, MN
tags: Microfluidics · Process Development · Biomedical Manufacturing
subtitle: "Flow-focusing microfluidic encapsulation scaled from fragile capsule generation into a throughput/yield operating-window problem."
---

<div class="selected-outcomes micro-stats-hero">
 <div class="metric-strip method-note-strip">
  <span class="stat-primary"><strong>20×</strong><em>throughput increase</em><small>Baseline: initial manual droplet generation rate. Measured: post-tooling-redesign flow rate.</small></span>
  <span class="stat-primary"><strong>~50%</strong><em>usable-yield improvement</em><small>Microscopy-counted usable capsule fraction, pre vs. post flow-ratio and crosslinking optimization.</small></span>
  <span class="stat-qual"><strong>Lower coalescence</strong><em>qualitative failure reduction</em></span>
  <span class="stat-qual"><strong>QC workflow</strong><em>microscopy-supported defect interpretation</em></span>
 </div>
</div>

<div class="thesis-box promoted-thesis-box">
 <h2>Faster capsule generation was only useful inside a usable operating window.</h2>
 <p>Increased capsule-generation throughput by 20× and improved microscopy-counted usable encapsulation yield by ~50% after flow-ratio, tooling, and crosslinking adjustments.</p>
</div>

<section class="artifact-panel public-safe-snapshot" aria-label="Operating-window summary">
 <h2>Process insight</h2>
 <p>Faster throughput was not automatically better. Speed only mattered when flow ratio, droplet formation, crosslink timing, and collection conditions stayed inside a usable operating window.</p>
</section>

## System

The system was a flow-focusing microfluidic process for generating core-shell hydrogel capsules containing stem cells. The engineering problem was not only generating droplets; it was generating capsules that remained usable after formation, crosslinking, collection, and microscopy inspection.

## Operating-window table

<div class="artifact-table-wrap">
<table class="artifact-table">
<thead><tr><th>Process change</th><th>Failure mode addressed</th><th>Metric affected</th><th>Result</th></tr></thead>
<tbody>
<tr><td>Flow-ratio tuning</td><td>Unstable capsule formation / coalescence</td><td>Usable yield</td><td>~50% improvement</td></tr>
<tr><td>Tooling redesign</td><td>Low generation rate</td><td>Throughput</td><td>20× increase</td></tr>
<tr><td>Crosslink timing adjustment</td><td>Fragile shells / post-formation instability</td><td>Handling stability</td><td>Improved usable capsule fraction</td></tr>
<tr><td>Microscopy QC</td><td>Unclassified defects</td><td>Yield interpretation</td><td>Defect classes became visible</td></tr>
</tbody>
</table>
</div>

<p class="method-note"><strong>Yield definition:</strong> usable yield refers to the microscopy-counted usable capsule fraction after excluding visibly coalesced, malformed, or otherwise defective capsules from the usable-capsule count.</p>

## What I measured

<div class="process-map compact-flow-map" aria-label="Microencapsulation metric flow">
 <div class="process-map-stage"><p>INPUTS</p><span>flow ratio</span><span>tooling geometry</span><span>crosslink timing</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage"><p>FAILURE MODES</p><span>coalescence</span><span>fragile shells</span><span>size variability</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage decision-stage"><p>OUTPUTS</p><span>throughput, usable yield, defect classes, run-to-run variability</span></div>
</div>

## Methods and tools

<div class="two-col">
 <div class="matrix-card"><h3>Process development</h3><p>Flow-focusing microfluidics, 3D-printed tooling, flow-ratio adjustment, crosslink automation, collection handling, and repeatability-focused process changes.</p></div>
 <div class="matrix-card"><h3>Measurement</h3><p>Microscopy inspection, capsule size interpretation, coalescence tracking, usable-yield counting, and run-to-run comparison.</p></div>
</div>

<div class="badge-row"><span class="badge">Flow focusing</span><span class="badge">Microfluidics</span><span class="badge">3D-printed tooling</span><span class="badge">Microscopy QC</span><span class="badge">Crosslinking</span><span class="badge">Mayo Clinic</span></div>

<div class="what-changed-block">
 <h2>What changed because of this</h2>
 <p>The project moved from trying to make capsules faster to defining which flow and crosslinking conditions made faster capsule generation usable.</p>
</div>

## What I’d do next

I would formalize the process window as a small response-surface study with throughput, usable yield, size distribution, and coalescence as CTQs. The engineering decision would be a recommended operating region, not a single “best” flow setting that fails when tooling, collection, or crosslinking conditions change.

<div class="case-cta-row">
 <a class="button primary" href="{{ '/projects/' | relative_url }}">View all case files</a>
 <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Download Resume</a>
 <a class="button tertiary" href="mailto:{{ site.email }}">Contact</a>
</div>
