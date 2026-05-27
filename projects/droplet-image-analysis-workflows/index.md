---
layout: page
title: Droplet Image Analysis Workflows
category: Image analysis · droplet metrics · Filler Lab · Georgia Tech
date_range: 2025–present
metric_chips: '<span>Video → CTQ</span><span>Segmentation workflow</span>'
description: Image-analysis case file turning microscopy videos into calibrated droplet traces, CTQs, and QC-ready measurement outputs.
subtitle: Microscopy-video workflows for converting droplet behavior into calibrated time-series outputs.
body_class: case-file-page
---

<section class="artifact-panel setup-snapshot">
 <h2>The setup</h2>
 <ul class="snapshot-list">
  <li><strong>System:</strong> microscopy videos of droplets used to compare wetting, contact-line motion, and deposition behavior.</li>
  <li><strong>Inputs handled:</strong> frame rate, pixel calibration, crop region, segmentation settings, and trace export format.</li>
  <li><strong>Outputs:</strong> normalized radius traces, contact-line classifications, QC notes, and export-ready tables for comparing runs.</li>
 </ul>
</section>
<section class="acronym-legend">
 <strong>Notation:</strong> <span><abbr title="Critical-to-Quality">CTQ</abbr> = measurable requirement the workflow has to deliver.</span> <span><abbr title="Design of Experiments">DOE</abbr> = structured run plan.</span> <span><abbr title="Failure Mode and Effects Analysis">FMEA</abbr> = failure-mode map used to prioritize checks.</span>
</section>

<section class="pipeline-card" aria-label="Image analysis pipeline">
 <h2>Raw video → calibration → object detection → track linking → radial/tangential decomposition → dashboard export</h2>
 <div class="mini-flow pipeline-flow"><span>Raw video</span><b>→</b><span>Calibration</span><b>→</b><span>Object detection</span><b>→</b><span>Track linking</span><b>→</b><span>Vector decomposition</span><b>→</b><span>Dashboard</span></div>
</section>

<section class="artifact-grid two-col-artifacts" aria-label="Droplet image-analysis artifacts">
 <article class="artifact-card">
  <span class="artifact-label">Dashboard</span>
  <div class="artifact-image-wrap"><img class="artifact-image" src="{{ '/assets/images/artifacts/group-motion-dashboard.png' | relative_url }}" alt="Group motion dashboard exported from microdevice tracking" loading="lazy"></div>
  <p class="artifact-caption"><strong>Group motion dashboard.</strong> Trajectory-linked detections are summarized as population speed, radial velocity, angular velocity tendency, and tracking coverage. This supports fast comparison of whether a run produces outward sweep, immobilization, or late-stage crowding.</p>
 </article>
 <article class="artifact-card">
  <span class="artifact-label">Velocity decomposition</span>
  <div class="artifact-image-wrap"><img class="artifact-image" src="{{ '/assets/images/artifacts/radial-tangential-velocity.png' | relative_url }}" alt="Radial and tangential velocity plots from tracked microdevices" loading="lazy"></div>
  <p class="artifact-caption"><strong>Radial and tangential velocity decomposition.</strong> Tracks are resolved relative to the droplet center so motion direction becomes a measurable process output, not just a visual impression.</p>
 </article>
 <article class="artifact-card code-artifact">
  <span class="artifact-label">Code / analysis excerpt</span>
  <div class="artifact-image-wrap code-image-wrap"><img class="artifact-image" src="{{ '/assets/images/artifacts/thermocycler-code-pid-crop.png' | relative_url }}" alt="Control-analysis code excerpt" loading="lazy"></div>
  <p class="artifact-caption"><strong>Control-analysis code excerpt.</strong> Experimental video or sensor data becomes structured process metrics through explicit state logic, filtering, and export behavior. Code screenshots stay secondary to plots and physical artifacts.</p>
 </article>
 <article class="artifact-card setup-artifact">
  <span class="artifact-label">Measurement setup</span>
  <div class="artifact-image-wrap"><img class="artifact-image" src="{{ '/assets/images/artifacts/rame-hart-goniometer-cropped.jpg' | relative_url }}" alt="Rame-Hart goniometer setup for droplet characterization" loading="lazy"></div>
  <p class="artifact-caption"><strong>Rame-Hart goniometer setup used for droplet shape, contact angle, and volume/time characterization.</strong> Use only as a setup image, not a flagship artifact.</p>
 </article>
</section>

<section class="artifact-panel setup-snapshot"><h2>What good looks like</h2><p>Raw microscopy videos are not metrics. The workflow turns frames into calibrated variables: droplet radius, contact-line motion, contact angle proxy, volume proxy, and deposition distribution.</p></section>

<section class="insight-block tone-dark"><p>A droplet video becomes an engineering artifact only after calibration, segmentation choices, and trace outputs are documented well enough to audit.</p></section>

<section class="quality-checklist-card">
 <h2>Quality-control checklist</h2>
 <ul class="checklist-grid">
  <li>pixel-to-micron calibration</li>
  <li>frame-rate verification</li>
  <li>track-loss filtering</li>
  <li>smoothing-window reporting</li>
  <li>sign convention for radial velocity</li>
  <li>tracking coverage over time</li>
  <li>replicate count by condition</li>
 </ul>
</section>

## What I'd do next

<div class="next-iteration-callout"><p>The next iteration should package the workflow into a reproducible tool: load video, confirm calibration, extract contact line, export standard plots, and save each processing choice. The engineering decision is whether a trace is trustworthy enough to compare across substrates.</p></div>

## Video-to-metric workflow

<div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Step</th><th>Output</th><th>Failure mode checked</th></tr></thead><tbody>
<tr><td>Frame extraction</td><td>Standard time base</td><td>Dropped frames or inconsistent sampling.</td></tr>
<tr><td>Calibration</td><td>Pixels to length</td><td>Wrong scale bar or cropped reference.</td></tr>
<tr><td>Segmentation</td><td>Droplet edge and ROI</td><td>Threshold artifact or poor contrast.</td></tr>
<tr><td>Trace extraction</td><td>r(t), normalized r(t), edge/center ratio</td><td>Metric dominated by image noise instead of physics.</td></tr>
</tbody></table></div>

## What this shifted

<div class="what-changed-block changed-panel"><p>The workflow made droplet comparison auditable. Conditions could be compared by extracted traces and deposition regions, not only by visually inspecting the final stain.</p></div>

<div class="case-cta-row two-button-cta">
 <a class="button primary" href="{{ '/projects/process-simulation-design/' | relative_url }}">Next: Process Simulation and Design →</a>
 <a class="button secondary email-button" href="mailto:{{ site.email }}">Email Nathan</a>
</div>
