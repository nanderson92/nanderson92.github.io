---
layout: page
title: Stem-Cell Microencapsulation
category: Microfluidics · Mayo Clinic · Rochester, MN
date_range: Summer 2025
last_updated: May 2026
metric_chips: '<span><strong>20×</strong> throughput increase</span><span><strong>~50%</strong> usable-yield improvement</span>'
description: Microfluidic stem-cell microencapsulation case file showing 20× throughput and ~50% usable-yield improvement through flow and tooling changes.
subtitle: Microfluidic capsule-generation work that made throughput useful by keeping yield and handling stability inside the operating window.
body_class: case-file-page
---

<section class="artifact-panel setup-snapshot">
 <h2>Setup</h2>
 <ul class="snapshot-list">
  <li><strong>System:</strong> flow-focusing microfluidic alginate-core / PEG-shell capsule generation for <abbr title="adult retinal pigment epithelial cell line">ARPE-19</abbr> cell culture.</li>
  <li><strong>Inputs adjusted:</strong> flow ratio, tooling geometry, shielding/crosslinking conditions, and collection workflow.</li>
  <li><strong>Measured outputs:</strong> capsule-generation rate, microscopy-counted usable yield, coalescence, shell integrity, and handling stability.</li>
  <li><strong>Result:</strong> increased capsule-generation throughput by 20× and improved microscopy-counted usable encapsulation yield by ~50% after flow-ratio, tooling, and crosslinking adjustments.</li>
 </ul>
</section>
<section class="acronym-legend">
 <strong>Notation:</strong> <span><abbr title="polyethylene glycol">PEG</abbr> = shell material.</span> <span><abbr title="adult retinal pigment epithelial cell line">ARPE-19</abbr> = retinal pigment epithelial cell line.</span> <span><abbr title="Critical-to-Quality">CTQ</abbr> = measurable requirement the workflow has to deliver.</span>
</section>

<section class="artifact-stack microencap-artifacts" aria-label="Stem-cell microencapsulation artifacts">
 <article class="artifact-card artifact-card-wide hero-artifact">
  <p class="artifact-label">MICROSCOPY</p>
  <figure class="artifact-figure">
   <div class="artifact-image-frame frame-microscopy"><img src="{{ '/assets/images/artifact-microcapsule-microscopy.jpg' | relative_url }}" alt="Representative hydrogel microcapsules under microscopy" loading="lazy"></div>
   <figcaption><strong>Figure 1. Representative hydrogel microcapsules from the microfluidic encapsulation workflow.</strong> The microscopy image shows capsule morphology and visual process output used for yield and quality assessment.</figcaption>
  </figure>
 </article>
 <article class="artifact-card artifact-card-wide">
  <p class="artifact-label">QUANTITATIVE OUTPUT</p>
  <figure class="artifact-figure">
   <div class="artifact-image-frame frame-chart"><img src="{{ '/assets/images/artifact-peg-shell-thickness.png' | relative_url }}" alt="PEG shell thickness versus shell flow rate chart" loading="lazy"></div>
   <figcaption><strong>Figure 2. PEG shell thickness as a function of shell flow rate.</strong> The project chart shows that process inputs shifted capsule structure. Statistical interpretation should be tied to the original run log, sample count, and error-bar definition.</figcaption>
  </figure>
 </article>
 <article class="artifact-card artifact-card-wide">
  <p class="artifact-label">MECHANISM SCHEMATIC</p>
  <figure class="artifact-figure">
   <div class="artifact-image-frame frame-schematic"><img src="{{ '/assets/images/artifact-alginate-hardening.png' | relative_url }}" alt="Alginate core hardening concept schematic" loading="lazy"></div>
   <figcaption><strong>Figure 3. Alginate-core hardening concept.</strong> Calcium-mediated crosslinking converts a liquid alginate core into a mechanically stabilized hydrogel core.</figcaption>
  </figure>
 </article>
</section>

<section class="insight-block tone-dark"><p>Faster capsule generation was only useful when flow ratio, droplet formation, crosslink timing, and collection stayed inside a usable operating window.</p></section>

<section id="process-levers" class="artifact-panel metric-before-after">
 <h2>Process levers</h2>
 <div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Process change</th><th>Failure mode addressed</th><th>Metric affected</th><th>Observed outcome</th></tr></thead><tbody>
<tr><td>Flow-ratio tuning</td><td>Unstable capsule formation / coalescence</td><td>Usable yield</td><td>~50% improvement in microscopy-counted usable yield.</td></tr>
<tr><td>Tooling redesign</td><td>Low generation rate</td><td>Throughput</td><td>20× increase in capsule-generation throughput.</td></tr>
<tr><td>Crosslink timing adjustment</td><td>Fragile shells / post-formation instability</td><td>Handling stability</td><td>Improved usable capsule fraction.</td></tr>
<tr><td>Microscopy QC</td><td>Unclassified defects</td><td>Yield interpretation</td><td>Coalesced, unstable, malformed, and handling-damaged capsules became easier to separate.</td></tr>
</tbody></table></div>
<p class="method-note"><strong>Yield definition:</strong> percent usable capsules after excluding coalesced, visibly defective, or handling-unstable capsules during microscopy QC.</p>
</section>

<section class="mini-flow-card"><h2>Capsule workflow</h2><div class="mini-flow"><span>Set flow ratio</span><b>→</b><span>Generate capsules</span><b>→</b><span>Crosslink</span><b>→</b><span>Microscopy QC</span><b>→</b><span>Classify usable yield</span></div></section>

## Next run

<div class="next-iteration-callout">
 <p>The next iteration should convert yield categories into a compact control plan: acceptable capsule morphology, coalescence limit, collection timing, and microscopy sampling cadence. The engineering decision is whether a faster run stays inside the usable-yield window without hiding new defect classes.</p>
</div>

## What changed

<div class="what-changed-block changed-panel">
 <p>The project moved from trying to make capsules faster to defining which flow and crosslinking conditions made faster capsule generation usable.</p>
</div>

<div class="case-cta-row two-button-cta">
 <a class="button primary" href="{{ '/projects/micromodular-deposition/' | relative_url }}">Next: Micromodular Electronics Deposition →</a>
 <a class="button secondary email-button" href="mailto:{{ site.email }}">Email Nathan</a>
</div>
