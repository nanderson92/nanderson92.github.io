---
layout: page
title: Stem-Cell Microencapsulation
category: Microfluidics · Mayo Clinic · Rochester, MN
date_range: Summer 2025
metric_chips: '<span><strong>20×</strong> throughput increase</span><span><strong>~50%</strong> usable-yield improvement</span>'
subtitle: Microfluidic capsule-generation work that made throughput useful by keeping yield and handling stability inside the operating window.
---

<section class="artifact-panel public-safe-snapshot">
 <h2>Public-safe experiment snapshot</h2>
 <ul class="snapshot-list">
  <li><strong>System:</strong> flow-focusing microfluidic alginate-core / PEG-shell capsule generation for ARPE-19 cell culture.</li>
  <li><strong>Inputs adjusted:</strong> flow ratio, tooling geometry, shielding/crosslinking conditions, and collection workflow.</li>
  <li><strong>Measured outputs:</strong> capsule-generation rate, microscopy-counted usable yield, coalescence, shell integrity, and handling stability.</li>
  <li><strong>Result:</strong> increased capsule-generation throughput by 20× and improved microscopy-counted usable encapsulation yield by ~50% after flow-ratio, tooling, and crosslinking adjustments.</li>
 </ul>
</section>

<section class="visual-artifact-grid" aria-label="Visual artifact slots">
 <figure><img src="{{ '/assets/images/artifact-measurement-plot.svg' | relative_url }}" alt="Microencapsulation measurement plot area" loading="lazy"><figcaption>Plot area for throughput, yield, flow ratio, or shell-thickness comparison.</figcaption></figure>
 <figure><img src="{{ '/assets/images/artifact-device-image.svg' | relative_url }}" alt="Capsule microscopy image area" loading="lazy"><figcaption>Image area for capsule microscopy, device photo, or QC view.</figcaption></figure>
 <figure><img src="{{ '/assets/images/microfluidic-flow-schematic.svg' | relative_url }}" alt="Microfluidic flow schematic" loading="lazy"><figcaption>Flow schematic area for device geometry, streams, and crosslinking steps.</figcaption></figure>
</section>

## Operating-window table

<div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Process change</th><th>Failure mode addressed</th><th>Metric affected</th><th>Result</th></tr></thead><tbody>
<tr><td>Flow-ratio tuning</td><td>Unstable capsule formation / coalescence</td><td>Usable yield</td><td>~50% improvement</td></tr>
<tr><td>Tooling redesign</td><td>Low generation rate</td><td>Throughput</td><td>20× increase</td></tr>
<tr><td>Crosslink timing adjustment</td><td>Fragile shells / post-formation instability</td><td>Handling stability</td><td>Improved usable capsule fraction</td></tr>
<tr><td>Microscopy QC</td><td>Unclassified defects</td><td>Yield interpretation</td><td>Defect classes became visible</td></tr>
</tbody></table></div>
<p class="method-note"><strong>Yield definition:</strong> percent usable capsules after excluding coalesced, visibly defective, or handling-unstable capsules during microscopy QC.</p>

## Strongest process insight

Faster throughput was not automatically better. Speed only mattered when flow ratio, droplet formation, crosslink timing, and collection conditions stayed inside a usable operating window.

## What changed because of this

<div class="what-changed-block changed-panel">
 <p>The project moved from trying to make capsules faster to defining which flow and crosslinking conditions made faster capsule generation usable.</p>
</div>

## Open questions / next iteration

<div class="next-iteration-callout">
 <p>The next iteration should convert yield categories into a simple control plan: acceptable capsule morphology, coalescence limit, collection timing, and microscopy sampling cadence. The engineering decision is whether a faster run stays inside the usable-yield window without hiding new defect classes.</p>
</div>


<div class="case-cta-row two-button-cta">
 <a class="button primary" href="{{ '/projects/' | relative_url }}">Next case file →</a>
 <a class="button secondary email-button" href="mailto:{{ site.email }}">Email Nathan</a>
</div>
