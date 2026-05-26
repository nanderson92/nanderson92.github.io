---
layout: page
title: Thermocycler Process Automation
date_range: Summer 2025
affiliation: Mayo Clinic · Rochester, MN
category: Thermal-control validation
tags: Automation · Embedded Control · qPCR · Diagnostics
subtitle: "A thermal cycling prototype organized around validation metrics: ramp rate, overshoot, settling time, hold stability, and cycle repeatability."
---

<div class="thesis-box promoted-thesis-box">
 <h2>A setpoint is meaningless unless the sample region experiences the intended thermal history.</h2>
 <p>The main engineering lesson was that sensor placement and thermal lag dominated apparent controller performance.</p>
</div>

<section class="artifact-panel public-safe-snapshot" aria-label="Prototype validation snapshot">
 <h2>Prototype validation snapshot</h2>
 <ul class="snapshot-list">
  <li><strong>Controlled variables:</strong> denaturation, annealing, and extension setpoints.</li>
  <li><strong>Logged variables:</strong> measured block temperature versus time.</li>
  <li><strong>CTQs:</strong> ramp rate, overshoot, settling time, hold stability, cycle-to-cycle repeatability.</li>
  <li><strong>Main engineering lesson:</strong> sensor placement and thermal lag dominated apparent controller performance.</li>
 </ul>
</section>

## Validation logic

The first control problem looked like a software problem, but the limiting issue was physical: sensor placement, thermal lag, and heat transfer through the block. Better tuning helped only after the hardware response was treated as part of the process.

<div class="artifact-table-wrap">
<table class="artifact-table">
<thead><tr><th>Metric</th><th>Why it matters</th><th>What it reveals</th></tr></thead>
<tbody>
<tr><td>Ramp rate</td><td>Determines cycle time.</td><td>Heating/cooling power and thermal coupling.</td></tr>
<tr><td>Overshoot</td><td>Can damage assay conditions.</td><td>Controller tuning and thermal lag.</td></tr>
<tr><td>Hold stability</td><td>Controls reaction consistency.</td><td>Sensor placement and heat distribution.</td></tr>
<tr><td>Cycle repeatability</td><td>Determines protocol reliability.</td><td>System drift and control robustness.</td></tr>
</tbody>
</table>
</div>

## Control architecture

<div class="process-map compact-flow-map" aria-label="Thermocycler control architecture">
 <div class="process-map-stage"><p>PROTOCOL</p><span>denaturation</span><span>annealing</span><span>extension</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage"><p>CONTROL</p><span>ESP32/Arduino</span><span>PID tuning</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage"><p>ACTUATION</p><span>heater</span><span>cooling fan</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage decision-stage"><p>VALIDATE</p><span>measured temperature-time profile vs. intended sample exposure</span></div>
</div>

## Hardware and tools

<div class="two-col">
 <div class="matrix-card"><h3>Hardware / control</h3><p>Embedded controller, temperature sensor feedback, heater/fan actuation, PID tuning, and thermal cycling scripts.</p></div>
 <div class="matrix-card"><h3>Validation</h3><p>Thermal profile logging, ramp-rate calculation, hold-stability checks, repeatability checks, and protocol comparison.</p></div>
</div>

<div class="badge-row"><span class="badge">ESP32</span><span class="badge">Arduino</span><span class="badge">PID Control</span><span class="badge">Sensors</span><span class="badge">RT-qPCR</span><span class="badge">Automation</span></div>

## Public-safe validation output

<div class="measured-performance-grid">
 <figure class="data-placeholder-figure wide-placeholder">
  <img src="{{ '/assets/images/placeholder-thermocycler-temperature-profile.svg' | relative_url }}" alt="Thermocycler temperature versus time profile with validation bands." loading="lazy">
  <figcaption>Temperature-time trace format with setpoint, measured temperature, overshoot, ramp rate, and hold-stability band.</figcaption>
 </figure>
 <div class="performance-fields">
  <h3>Fields to extract from prototype logs</h3>
  <ul>
   <li><strong>Ramp rate:</strong> measured °C/s or °C/min between setpoints.</li>
   <li><strong>Overshoot:</strong> maximum excursion above each hold temperature.</li>
   <li><strong>Hold stability:</strong> temperature band during denaturation, annealing, and extension holds.</li>
   <li><strong>Repeatability:</strong> cycle-to-cycle variation across repeated thermal cycles.</li>
  </ul>
 </div>
</div>

<div class="what-changed-block">
 <h2>What changed because of this</h2>
 <p>The project taught me to treat temperature control as a validation problem, not just a code/hardware problem: a setpoint is meaningless unless the sample region actually experiences the intended thermal history.</p>
</div>

## What I’d do next

The next version would measure closer to the actual sample, not just the thermal block. I would also design the controller around the slowest physical response in the system instead of only chasing faster setpoint tracking, because overshoot that looks acceptable on the block can still be bad for the assay.

<div class="case-cta-row">
 <a class="button primary" href="{{ '/projects/' | relative_url }}">View all case files</a>
 <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Download Resume</a>
 <a class="button tertiary" href="mailto:{{ site.email }}">Contact</a>
</div>
