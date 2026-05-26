---
layout: page
title: Micromodular Electronics Deposition
category: Wet processing · printed electronics · Filler Lab · Georgia Tech
date_range: 2025–present
metric_chips: '<span>Screening framework</span><span>Image-derived droplet CTQs</span>'
subtitle: Substrate/backing screens for IPA droplet deposition of suspended microdevices before printed interconnect routing.
---

<section class="artifact-panel public-safe-snapshot">
 <h2>Public-safe experiment snapshot</h2>
 <ul class="snapshot-list">
  <li><strong>System:</strong> IPA droplet deposition of suspended microdevices on substrate/backing candidates.</li>
  <li><strong>Inputs varied:</strong> substrate, backing condition, droplet volume, and particle/device loading state.</li>
  <li><strong>Metrics extracted:</strong> r(t)/r0, contact-line regime, edge/center device ratio, qualitative repeatability, and final deposition pattern.</li>
  <li><strong>Current decision:</strong> prioritize porous AAO-like drainage conditions over glass-like evaporation controls.</li>
  <li><strong>Next threshold needed:</strong> replicate-backed edge/center ratio plus density uniformity target before interconnect printing.</li>
 </ul>
</section>


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


<section class="ownership-callout ownership-callout-large">
 <p>I designed the experiments from scratch: substrate/backing comparisons, top-view and side-view video capture, Python/ImageJ analysis, and placement metrics tied to downstream interconnect feasibility.</p>
</section>

## Useful placement definition

Useful placement means lower edge crowding, better center/field distribution, enough local density for downstream interconnect routing, repeatable final pattern, and a substrate/backing condition that can scale beyond brittle AAO coupons.

## Decision framework

<div class="decision-grid">
 <div class="decision-card pass-card">
  <h3>Candidate passes early screen if</h3>
  <ol>
   <li>Contact-line history can be classified from video.</li>
   <li>Edge/center device ratio improves relative to a glass-like evaporation control.</li>
   <li>Device density remains high enough for interconnect routing.</li>
   <li>Pattern is repeatable across replicate droplets.</li>
   <li>Substrate/backing condition is physically scalable beyond brittle AAO.</li>
  </ol>
 </div>
 <div class="decision-card fail-card">
  <h3>Candidate fails if</h3>
  <ul>
   <li>Fast liquid removal still creates edge-heavy crowding.</li>
   <li>Droplet footprint becomes too small or irregular for routing.</li>
   <li>Device rafts or pins unpredictably.</li>
   <li>Metric extraction cannot distinguish mechanism from artifact.</li>
  </ul>
 </div>
</div>

## My role

<div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Area</th><th>Contribution</th></tr></thead><tbody>
<tr><td>Experimental design</td><td>Substrate/backing comparisons, droplet setup, run-to-run comparison, and early screen logic.</td></tr>
<tr><td>Imaging</td><td>Top-view and side-view capture for footprint, contact-line, and final placement behavior.</td></tr>
<tr><td>Analysis</td><td>Python/ImageJ extraction of normalized contact-line traces and deposition metrics.</td></tr>
<tr><td>Decision output</td><td>Screening logic for substrate candidates before downstream interconnect printing.</td></tr>
</tbody></table></div>

## What changed because of this

<div class="what-changed-block changed-panel">
 <p>This work shifted the project from judging substrates by final visual stains to screening them by video-derived contact-line behavior, drainage/evaporation signatures, and placement metrics tied to interconnect feasibility.</p>
</div>

## Open questions / next iteration

<div class="next-iteration-callout">
 <p>The next iteration should set a replicate-backed edge/center ratio and density-uniformity threshold, then compare AAO-like skins against cheaper and less brittle porous supports. The engineering decision is whether the substrate can preserve placement while remaining compatible with downstream interconnect routing.</p>
</div>


<div class="case-cta-row two-button-cta">
 <a class="button primary" href="{{ '/projects/' | relative_url }}">Next case file →</a>
 <a class="button secondary email-button" href="mailto:{{ site.email }}">Email Nathan</a>
</div>
