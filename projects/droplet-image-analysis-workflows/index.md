---
layout: page
title: Droplet Image Analysis Workflows
category: Image analysis · droplet CTQs · 2025–present
date_range: 2025–present
tags: Image Analysis · Wet Processing · Python · Experimental Data
subtitle: "Converting droplet videos into radius traces, motion metrics, and deposition-bias variables."
---

<div class="metric-chip-row"><span class="metric-chip"><strong>r(t)</strong> extraction</span><span class="metric-chip"><strong>Motion</strong> metrics</span></div>

<section class="artifact-gallery" aria-label="Project artifact panels">
 <figure class="casefile-artifact"><img src="{{ '/assets/images/preliminary-radius-plot.svg' | relative_url }}" alt="Preliminary radius plot"><figcaption>Measurement plot panel: normalized contact-line trace.</figcaption></figure>
 <figure class="casefile-artifact"><img src="{{ '/assets/images/droplet-metric-panel.svg' | relative_url }}" alt="Droplet metric panel"><figcaption>Device/image panel: droplet frame and extracted geometry.</figcaption></figure>
 <figure class="casefile-artifact"><img src="{{ '/assets/images/artifact-flow-schematic.svg' | relative_url }}" alt="image-analysis workflow schematic"><figcaption>Flow schematic panel: video input, segmentation, trace extraction, metric table.</figcaption></figure>
</section>

<div class="thesis-box"><h2>Video becomes engineering evidence only after calibration and classification.</h2><p>The workflow extracts radius traces, device motion, radial drift, and deposition bias so surfaces can be compared without relying on visual impressions.</p></div>

## CTQ extraction plan

| Output | Method | Engineering use |
|---|---|---|
| r(t)/r0 | Top-view edge detection and calibration | Compare spreading and recession regimes. |
| Radial drift | Device centroid tracking relative to droplet center | Identify edgeward transport and raft behavior. |
| Velocity/acceleration | Time derivative of tracked position | Separate smooth advection from abrupt pinning. |
| Edge/center ratio | Final pattern segmentation | Quantify placement bias for routing feasibility. |

<div class="changed-panel"><h2>What changed because of this</h2><p>The deposition project gained an analysis layer that can separate contact-line behavior, particle motion, and final placement pattern instead of compressing everything into one final image.</p></div>

<div class="next-panel"><h2>Open questions / next iteration</h2><p>The next iteration is to lock image calibration, lighting, and segmentation thresholds before adding more substrates. That prevents the analysis pipeline from becoming a hidden experimental variable.</p></div>

<div class="cta-row bottom-case-cta"><a class="button primary" href="{{ '/projects/process-simulation-design/' | relative_url }}">Next case file →</a><a class="button secondary email-button" href="mailto:{{ site.email }}">Email Nathan</a></div>
