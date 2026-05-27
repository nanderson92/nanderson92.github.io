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



<section class="artifact-panel setup-snapshot"><h2>What good looks like</h2><p>Raw microscopy videos are not metrics. The workflow turns frames into calibrated variables: droplet radius, contact-line motion, contact angle proxy, volume proxy, and deposition distribution.</p></section>




<section class="insight-block tone-dark"><p>A droplet video becomes an engineering artifact only after calibration, segmentation choices, and trace outputs are documented well enough to audit.</p></section>

<section class="mini-flow-card"><h2>Analysis flow</h2><div class="mini-flow"><span>Video</span><b>→</b><span>Calibration</span><b>→</b><span>Segmentation</span><b>→</b><span>Trace extraction</span><b>→</b><span>QC export</span></div></section>

## What I'd do next

<div class="next-iteration-callout"><p>The next iteration should package the workflow into a reproducible tool: load video, confirm calibration, extract contact line, export standard plots, and save each processing choice. The engineering decision is whether a trace is trustworthy enough to compare across substrates.</p></div>

<section class="visual-artifact-grid" aria-label="Visual artifact slots">
 <figure>
  <img src="{{ '/assets/images/artifact-measurement-plot.svg' | relative_url }}" alt="Measurement plot artifact area" loading="lazy">
  <figcaption>Artifact placeholder — replace with a real measurement plot, trace, histogram, or validation curve.</figcaption>
 </figure>
 <figure>
  <img src="{{ '/assets/images/artifact-device-image.svg' | relative_url }}" alt="Device or microscopy image artifact area" loading="lazy">
  <figcaption>Artifact placeholder — replace with a real lab, microscope, device, capsule, printed-line, or run photo.</figcaption>
 </figure>
 <figure>
  <img src="{{ '/assets/images/artifact-flow-schematic.svg' | relative_url }}" alt="Flow or schematic artifact area" loading="lazy">
  <figcaption>Artifact placeholder — replace with a real screen, workflow, setup schematic, or control-logic diagram.</figcaption>
 </figure>
</section>

<section class="artifact-link-slot">
 <strong>External artifact slot</strong>
 <span>Artifact placeholder — add a real poster, GitHub notebook, PDF memo, slide, or shareable writeup link when available.</span>
</section>

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
