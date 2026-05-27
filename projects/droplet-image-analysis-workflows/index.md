---
layout: page
title: Droplet Image Analysis Workflows
category: Image analysis · droplet metrics · Filler Lab · Georgia Tech
date_range: 2025–present
metric_chips: '<span>Video → CTQ</span><span>Segmentation workflow</span>'
subtitle: Microscopy-video workflows for converting droplet behavior into calibrated time-series outputs.
meta_description: Case file on droplet image analysis workflows for converting microscopy videos into calibrated process metrics.
---

<section class="artifact-panel setup-panel"><h2>The setup</h2><p>Raw microscopy videos are not metrics. The workflow turns frames into calibrated variables: droplet radius, contact-line motion, contact angle proxy, volume proxy, and deposition distribution.</p></section>
<section class="insight-block dark-section"><p>A trace is only useful when calibration, segmentation choices, and noise checks are recorded with it.</p></section>
<section class="next-iteration-callout early-next"><h2>What I’d do next</h2><p>Package the workflow into a reproducible tool: load video, confirm calibration, extract contact line, export standard plots, and save each processing choice. The decision is whether a trace is trustworthy enough to compare across substrates.</p></section>
<section class="visual-artifact-grid" aria-label="Artifact placeholders">
 <figure><img src="{{ '/assets/images/artifact-measurement-plot.svg' | relative_url }}" alt="Chart artifact placeholder" loading="lazy"><figcaption><strong>Artifact placeholder:</strong> replace with the real chart, graph, trace, or distribution.</figcaption></figure>
 <figure><img src="{{ '/assets/images/artifact-device-image.svg' | relative_url }}" alt="Lab or microscopy artifact placeholder" loading="lazy"><figcaption><strong>Artifact placeholder:</strong> replace with the real lab photo, microscopy still, device image, or run image.</figcaption></figure>
 <figure><img src="{{ '/assets/images/artifact-flow-schematic.svg' | relative_url }}" alt="Code, analysis, or process-flow artifact placeholder" loading="lazy"><figcaption><strong>Artifact placeholder:</strong> replace with code snippet, analysis workflow, control plan, or schematic.</figcaption></figure>
</section>
<h2>Process levers</h2><div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Step</th><th>Output</th><th>Failure mode checked</th></tr></thead><tbody><tr><td>Frame extraction</td><td>Standard time base</td><td>Dropped frames or inconsistent sampling.</td></tr><tr><td>Calibration</td><td>Pixels to length</td><td>Wrong scale bar or cropped reference.</td></tr><tr><td>Segmentation</td><td>Droplet edge and ROI</td><td>Threshold artifact or poor contrast.</td></tr><tr><td>Trace extraction</td><td>r(t), normalized r(t), edge/center ratio</td><td>Metric dominated by image noise instead of physics.</td></tr></tbody></table></div>
<section class="what-changed-block changed-panel"><h2>What this shifted</h2><p>The work made the system easier to judge because the output was tied to a variable, a check, and a next action.</p></section>
<div class="case-cta-row two-button-cta"><a class="button primary" href="{{ '/projects/process-simulation-design/' | relative_url }}">Next: Engineering Case Files →</a><a class="button secondary email-button" href="mailto:{{ site.email }}">Email Nathan</a></div>
