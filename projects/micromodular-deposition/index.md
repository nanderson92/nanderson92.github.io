---
layout: page
title: Micromodular Electronics Deposition
category: Wet processing · printed electronics · Filler Lab · Georgia Tech
date_range: 2025–present
metric_chips: '<span>Screening framework</span><span>Image-derived droplet CTQs</span>'
description: Substrate and backing screens for IPA droplet deposition of suspended microdevices, using video-derived droplet CTQs and placement metrics.
subtitle: Substrate/backing screens for <abbr title="isopropyl alcohol">IPA</abbr> droplet deposition of suspended microdevices before printed interconnect routing.
body_class: case-file-page
---

<section class="artifact-panel setup-snapshot">
 <h2>The setup</h2>
 <ul class="snapshot-list">
  <li><strong>System:</strong> <abbr title="isopropyl alcohol">IPA</abbr> droplet deposition of suspended microdevices on substrate/backing candidates.</li>
  <li><strong>Inputs varied:</strong> substrate, backing condition, droplet volume, and particle/device loading state.</li>
  <li><strong>Metrics extracted:</strong> <abbr title="droplet radius as a function of time, normalized by initial radius">r(t)/r0</abbr>, contact-line regime, edge/center device ratio, qualitative repeatability, and final deposition pattern.</li>
  <li><strong>Current decision:</strong> prioritize porous <abbr title="anodic aluminum oxide">AAO</abbr>-like drainage conditions over glass-like evaporation controls.</li>
  <li><strong>Next threshold needed:</strong> replicate-backed edge/center ratio plus density uniformity target before interconnect printing.</li>
 </ul>
</section>
<section class="acronym-legend">
 <strong>Notation:</strong> <span><abbr title="Critical-to-Quality">CTQ</abbr> = measurable requirement the workflow has to deliver.</span> <span><abbr title="Design of Experiments">DOE</abbr> = structured run plan.</span> <span><abbr title="Failure Mode and Effects Analysis">FMEA</abbr> = failure-mode map used to prioritize checks.</span>
</section>





<section class="insight-block tone-dark"><p>Boundary conditions controlled the outcome more than the final stain suggested. The deposition problem became a screen for contact-line history, drainage signature, and interconnect-accessible placement.</p></section>

<section class="mini-flow-card"><h2>Screen flow</h2><div class="mini-flow"><span>Prepare substrate/backing</span><b>→</b><span>Deposit droplet</span><b>→</b><span>Extract r(t)</span><b>→</b><span>Score placement</span><b>→</b><span>Pick next condition</span></div></section>

## What I'd do next

<div class="next-iteration-callout">
 <p>The next iteration should set a replicate-backed edge/center ratio and density-uniformity threshold, then compare AAO-like skins against cheaper and less brittle porous supports. The engineering decision is whether the substrate can preserve placement while remaining compatible with downstream interconnect routing.</p>
</div>

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



<section class="ownership-callout ownership-callout-large">
 <p>I designed the experiments from scratch: substrate/backing comparisons, top-view and side-view video capture, Python/ImageJ analysis, and placement metrics tied to downstream interconnect feasibility.</p>
</section>

## What good looks like

Good deposition means uniform areal density, low edge bias, usable placement for downstream interconnects, repeatable droplet behavior, and substrate compatibility with scale-up. Useful placement means lower edge crowding, better center/field distribution, enough local density for downstream interconnect routing, repeatable final pattern, and a substrate/backing condition that can scale beyond brittle AAO coupons.

## Pass / fail criteria

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
  <ol>
   <li>Fast liquid removal still creates edge-heavy crowding.</li>
   <li>Droplet footprint becomes too small or irregular for routing.</li>
   <li>Device rafts or pins unpredictably.</li>
   <li>Metric extraction cannot distinguish mechanism from artifact.</li>
  </ol>
 </div>
</div>

## What I owned

<div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Area</th><th>Contribution</th></tr></thead><tbody>
<tr><td>Experimental design</td><td>Substrate/backing comparisons, droplet setup, run-to-run comparison, and early screen logic.</td></tr>
<tr><td>Imaging</td><td>Top-view and side-view capture for footprint, contact-line, and final placement behavior.</td></tr>
<tr><td>Analysis</td><td>Python/ImageJ extraction of normalized contact-line traces and deposition metrics.</td></tr>
<tr><td>Decision output</td><td>Screening logic for substrate candidates before downstream interconnect printing.</td></tr>
</tbody></table></div>

## What this shifted

<div class="what-changed-block changed-panel">
 <p>This work shifted the project from judging substrates by final visual stains to screening them by video-derived contact-line behavior, drainage/evaporation signatures, and placement metrics tied to interconnect feasibility.</p>
</div>


<div class="case-cta-row two-button-cta">
 <a class="button primary" href="{{ '/projects/microencapsulation-process-development/' | relative_url }}">Next: Stem-Cell Microencapsulation →</a>
 <a class="button secondary email-button" href="mailto:{{ site.email }}">Email Nathan</a>
</div>
