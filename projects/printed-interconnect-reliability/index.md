---
layout: page
title: Printed Interconnect Reliability
category: Resistance drift → failure logic
date_range: 2025–present
affiliation: Filler Lab, Georgia Institute of Technology
tags: Printed Electronics · Reliability · Electrical Testing · Process Feedback
subtitle: "A public-safe reliability screen for turning printed-interconnect resistance behavior into pass, monitor, fail, or artifact decisions."
---

<div class="thesis-box promoted-thesis-box">
 <h2>Time-zero function and process robustness are not the same thing.</h2>
 <p>A printed interconnect can pass an initial check and still carry vulnerability from geometry, cure, material aging, humidity sensitivity, probe artifact, or handling damage.</p>
</div>

<section class="artifact-panel public-safe-snapshot" aria-label="Reliability screen skeleton">
 <h2>Reliability screen skeleton</h2>
 <ol class="snapshot-list ordered-snapshot">
  <li>Measure initial resistance after print/cure.</li>
  <li>Normalize resistance to baseline.</li>
  <li>Apply stress interval.</li>
  <li>Re-measure at defined time points.</li>
  <li>Classify trace as pass / monitor / fail / artifact.</li>
  <li>Map failure class to candidate upstream process cause.</li>
 </ol>
</section>

## Measurement context

The reliability work connects electrical outputs to process history. The measurement stack includes four-point probe resistance checks, Keithley SMU Id–Vg / Id–Vd sweeps for printed microdevice performance validation, microscopy inspection, stress intervals, and resistance-drift / failure-timing interpretation.

## Failure-decision table

<div class="artifact-table-wrap">
<table class="artifact-table failure-table">
<thead><tr><th>Failure class</th><th>What it suggests</th><th>Upstream process check</th></tr></thead>
<tbody>
<tr><td>High initial resistance</td><td>Poor print continuity, geometry, or cure.</td><td>Inspect line shape, cure, deposition continuity, and probe placement.</td></tr>
<tr><td>Smooth upward drift</td><td>Material aging or environmental sensitivity.</td><td>Check humidity exposure, sintering/cure condition, and material stability.</td></tr>
<tr><td>Sudden open circuit</td><td>Cracking, delamination, or handling damage.</td><td>Inspect physical damage, substrate handling, and probe history.</td></tr>
<tr><td>Intermittent readings</td><td>Contact artifact or true instability.</td><td>Separate probe/contact artifact from line failure through retest logic.</td></tr>
</tbody>
</table>
</div>

## Threshold logic

<div class="decision-grid reliability-threshold-grid">
 <article class="decision-card pass-card"><h3>Pass</h3><p>Initial resistance and drift stay inside the accepted screen window for the intended use case.</p></article>
 <article class="decision-card"><h3>Monitor</h3><p>Resistance remains functional but drift or variability suggests process-built vulnerability.</p></article>
 <article class="decision-card fail-card"><h3>Fail</h3><p>Trace crosses the defined resistance/failure state or shows nonrecoverable open-circuit behavior.</p></article>
 <article class="decision-card"><h3>Artifact / retest</h3><p>Signal changes are plausibly caused by probe contact, handling, or measurement setup rather than the printed line.</p></article>
</div>

## Process-feedback loop

<div class="process-map compact-flow-map" aria-label="Reliability feedback loop">
 <div class="process-map-stage"><p>MEASURE</p><span>4-point probe</span><span>Keithley sweeps</span><span>microscopy</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage"><p>CLASSIFY</p><span>initial resistance</span><span>drift</span><span>failure timing</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage decision-stage"><p>CHECK UPSTREAM</p><span>print continuity, cure, geometry, material stability</span></div>
</div>

## Methods and tools

<div class="two-col">
 <div class="matrix-card"><h3>Electrical testing</h3><p>Four-point probe measurements, Keithley SMU Id–Vg / Id–Vd sweeps, baseline normalization, stress intervals, and resistance-drift interpretation.</p></div>
 <div class="matrix-card"><h3>Process linkage</h3><p>Connect failure timing to possible upstream contributors: print geometry, cure/sintering condition, environmental exposure, handling, and measurement artifact.</p></div>
</div>

<div class="badge-row"><span class="badge">Four-point probe</span><span class="badge">Keithley SMU</span><span class="badge">Resistance drift</span><span class="badge">Stress intervals</span><span class="badge">Failure timing</span><span class="badge">Microscopy</span></div>

<div class="what-changed-block">
 <h2>What changed because of this</h2>
 <p>This work reframed interconnect testing from a time-zero pass/fail check into a reliability screen that can identify process-built vulnerability before full device failure.</p>
</div>

## What I’d do next

I would turn the public-safe failure classes into a formal control-plan draft: sampling frequency, stress interval, retest rule, and upstream corrective-action owner. The decision would be whether a line is stable enough for routing validation, needs monitoring, or should trigger a print/cure process check before more devices are consumed.

<div class="case-cta-row">
 <a class="button primary" href="{{ '/projects/micromodular-deposition/' | relative_url }}">Related deposition case →</a>
 <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Download Resume</a>
 <a class="button tertiary" href="mailto:{{ site.email }}">Contact</a>
</div>
