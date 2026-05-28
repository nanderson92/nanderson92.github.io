---
layout: page
title: Droplet Image Analysis Workflows
category: Image analysis · droplet metrics · Filler Lab · Georgia Tech
date_range: 2025–present
last_updated: May 2026
prev_title: Thin-Film Characterization-to-Process Logic
prev_url: /projects/thin-film-semiconductor-research/
next_title: Stem-Cell Microencapsulation
next_url: /projects/microencapsulation-process-development/
metric_chips: '<span>Video → metric</span><span>Segmentation workflow</span>'
description: Image-analysis case file turning microscopy videos into calibrated droplet traces, critical-to-quality measurement notes, and QC-ready outputs.
subtitle: Microscopy-video workflows for converting droplet behavior into calibrated time-series outputs.
body_class: case-file-page droplet-image-analysis-workflows
affiliation: Filler Lab · Georgia Tech
---

<section class="analysis-pipeline-card lead-pipeline-card">
 <p class="artifact-label">METHOD PIPELINE</p>
 <h2>Raw video → calibration → object detection → track linking → radial/tangential decomposition → dashboard export</h2>
 <p>The workflow turns microscopy frames into auditable process metrics, so runs can be compared by motion, coverage, and deposition behavior instead of visual impression alone.</p>
</section>

<section class="artifact-grid artifact-grid-two" aria-label="Droplet image analysis artifacts">
 <article class="artifact-card artifact-card-wide full-span-artifact">
  <p class="artifact-label">RAW → PROCESSED</p>
  <figure class="artifact-figure">
   <div class="artifact-image-frame frame-wide"><img src="{{ '/assets/images/droplet-raw-to-processed-pair.webp' | relative_url }}" alt="Raw microscope frame paired with processed trajectory overlay" loading="lazy"></div>
   <figcaption><strong>Figure 1. Raw frame to processed trajectory artifact.</strong> A raw microscope frame is paired with the extracted pathlines so object detection, track linking, and transport metrics can be checked instead of treated as a black box.</figcaption>
  </figure>
 </article>
 <article class="artifact-card artifact-card-wide">
  <p class="artifact-label">DASHBOARD EXPORT</p>
  <figure class="artifact-figure">
   <div class="artifact-image-frame frame-dashboard"><img src="{{ '/assets/images/artifact-group-motion-dashboard-1400.webp' | relative_url }}" alt="Group motion dashboard exported from tracked microdevice trajectories" loading="lazy"></div>
   <figcaption><strong>Figure 2. Group motion dashboard from tracked microdevice trajectories.</strong> Population speed, radial velocity, angular-velocity tendency, and tracking coverage are plotted against time. This supports condition-to-condition comparison and flags intervals where tracking coverage may bias the metric.</figcaption>
  </figure>
 </article>
 <article class="artifact-card artifact-card-wide">
  <p class="artifact-label">VELOCITY DECOMPOSITION</p>
  <figure class="artifact-figure">
   <div class="artifact-image-frame frame-plot"><img src="{{ '/assets/images/artifact-radial-tangential-velocity.png' | relative_url }}" alt="Radial and tangential velocity decomposition from droplet video" loading="lazy"></div>
   <figcaption><strong>Figure 3. Radial and tangential velocity decomposition.</strong> Tracks are resolved relative to the droplet center so outward transport and circumferential drift can be separated. This supports substrate/backing screens where final placement alone hides the transport path.</figcaption>
  </figure>
 </article>
 <article class="artifact-card setup-artifact-card">
  <p class="artifact-label">MEASUREMENT SETUP</p>
  <figure class="artifact-figure">
   <div class="artifact-image-frame frame-photo"><img src="{{ '/assets/images/artifact-rame-hart-goniometer-cropped.webp' | relative_url }}" alt="Cropped Rame-Hart goniometer setup" loading="lazy"></div>
   <figcaption><strong>Figure 4. Rame-Hart goniometer setup.</strong> Setup image for droplet shape, contact angle, and volume/time characterization.</figcaption>
  </figure>
 </article>
</section>

<section class="artifact-panel setup-snapshot">
 <h2>Setup</h2>
 <ul class="snapshot-list">
  <li><strong>System:</strong> microscopy videos of droplets used to compare wetting, contact-line motion, and deposition behavior.</li>
  <li><strong>Inputs handled:</strong> frame rate, pixel calibration, crop region, segmentation settings, and trace export format.</li>
  <li><strong>Outputs:</strong> normalized radius traces, contact-line classifications, critical-to-quality measurement notes, and export-ready tables for comparing runs.</li>
 </ul>
</section>

<section class="insight-block tone-dark"><p>A droplet video becomes an engineering artifact only after calibration, segmentation choices, and trace outputs are documented well enough to audit.</p></section>

<section class="artifact-panel qc-checklist-panel">
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

## Video-to-metric workflow

<div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Step</th><th>Output</th><th>Failure mode checked</th></tr></thead><tbody>
<tr><td>Frame extraction</td><td>Standard time base</td><td>Dropped frames or inconsistent sampling.</td></tr>
<tr><td>Calibration</td><td>Pixels to length</td><td>Wrong scale bar or cropped reference.</td></tr>
<tr><td>Segmentation</td><td>Droplet edge and ROI</td><td>Threshold artifact or poor contrast.</td></tr>
<tr><td>Trace extraction</td><td>radius trace, normalized radius trace, edge/center ratio</td><td>Metric dominated by image noise instead of physics.</td></tr>
</tbody></table></div>

## Next run

<div class="next-iteration-callout"><p>The next iteration should package the workflow into a reproducible tool: load video, confirm calibration, extract contact line, export standard plots, and save each processing choice. The engineering decision is whether a trace is trustworthy enough to compare across substrates.</p></div>

## What changed

<div class="what-changed-block changed-panel"><p>The workflow made droplet comparison auditable. Conditions could be compared by extracted traces and deposition regions, not only by visually inspecting the final stain.</p></div>

<div class="case-cta-row two-button-cta">
 <a class="button primary" href="{{ '/projects/microencapsulation-process-development/' | relative_url }}">Next: Stem-Cell Microencapsulation →</a>
 <a class="button secondary email-button" href="mailto:{{ site.email }}?subject=Droplet%20analysis%20case%20file">Email Nathan</a>
</div>
