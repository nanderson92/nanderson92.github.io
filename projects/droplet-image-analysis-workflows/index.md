---
layout: page
title: Droplet Image Analysis Workflows
category: Image analysis · droplet metrics · Filler Lab · Georgia Tech
date_range: 2025–present
metric_chips: '<span>Video → CTQ</span><span>Segmentation workflow</span>'
subtitle: Microscopy-video workflows for converting droplet behavior into calibrated time-series outputs.
---

<section class="artifact-panel public-safe-snapshot"><h2>Workflow objective</h2><p>Raw microscopy videos are not metrics. The workflow turns frames into calibrated variables: droplet radius, contact-line motion, contact angle proxy, volume proxy, and deposition distribution.</p></section>


<section class="visual-artifact-grid" aria-label="Visual artifact slots">
 <figure>
  <img src="{{ '/assets/images/artifact-measurement-plot.svg' | relative_url }}" alt="Measurement plot artifact area" loading="lazy">
  <figcaption>Measurement plot area for the real experimental trace, histogram, or validation curve.</figcaption>
 </figure>
 <figure>
  <img src="{{ '/assets/images/artifact-device-image.svg' | relative_url }}" alt="Device or microscopy image artifact area" loading="lazy">
  <figcaption>Image area for microscopy, device, capsule, printed-line, or run photo.</figcaption>
 </figure>
 <figure>
  <img src="{{ '/assets/images/artifact-flow-schematic.svg' | relative_url }}" alt="Flow or schematic artifact area" loading="lazy">
  <figcaption>Schematic area for the screen, workflow, or control logic.</figcaption>
 </figure>
</section>


## Video-to-metric workflow

<div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Step</th><th>Output</th><th>Failure mode checked</th></tr></thead><tbody>
<tr><td>Frame extraction</td><td>Standard time base</td><td>Dropped frames or inconsistent sampling.</td></tr>
<tr><td>Calibration</td><td>Pixels to length</td><td>Wrong scale bar or cropped reference.</td></tr>
<tr><td>Segmentation</td><td>Droplet edge and ROI</td><td>Threshold artifact or poor contrast.</td></tr>
<tr><td>Trace extraction</td><td>r(t), normalized r(t), edge/center ratio</td><td>Metric dominated by image noise instead of physics.</td></tr>
</tbody></table></div>

## What changed because of this

<div class="what-changed-block changed-panel"><p>The workflow made droplet comparison auditable. Conditions could be compared by extracted traces and deposition regions, not only by visually inspecting the final stain.</p></div>

## Open questions / next iteration

<div class="next-iteration-callout"><p>The next iteration should package the workflow into a reproducible tool: load video, confirm calibration, extract contact line, export standard plots, and save each processing choice. The engineering decision is whether a trace is trustworthy enough to compare across substrates.</p></div>


<div class="case-cta-row two-button-cta">
 <a class="button primary" href="{{ '/projects/' | relative_url }}">Next case file →</a>
 <a class="button secondary email-button" href="mailto:{{ site.email }}">Email Nathan</a>
</div>
