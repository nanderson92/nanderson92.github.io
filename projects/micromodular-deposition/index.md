---
layout: page
title: Micromodular Electronics Deposition
category: Wet processing · printed electronics · Filler Lab · Georgia Tech
date_range: 2025–present
last_updated: May 2026
prev_title: Stem-Cell Microencapsulation
prev_url: /projects/microencapsulation-process-development/
next_title: Printed Interconnect Reliability
next_url: /projects/printed-interconnect-reliability/
metric_chips: '<span>Screening framework</span><span>Image-derived droplet quality metrics</span>'
description: Substrate and backing screens for IPA droplet deposition of suspended microdevices, using image-derived droplet quality metrics and placement metrics.
subtitle: Substrate/backing screens for isopropyl alcohol (IPA) droplet deposition of suspended microdevices before printed interconnect routing.
body_class: case-file-page micromodular-deposition
affiliation: Filler Lab · Georgia Tech
---


<section class="artifact-panel micromodular-roadmap-overview" aria-label="Micromodular electronics roadmap">
 <div class="roadmap-overview-copy">
  <p class="artifact-label">SYSTEM ROADMAP</p>
  <h2>Where the deposition screen fits</h2>
  <p>The larger process is to fabricate discrete micromodular components, suspend them in an ink, print them into circuit locations, then analyze placement and route printed interconnects.</p>
  <p>This case file focuses on the deposition step: choosing substrate/backing conditions that place suspended components in a pattern downstream wiring can actually use. The screen is structured as design-of-experiments (DOE) thinking: vary the substrate/backing condition, measure placement outputs, and decide whether the condition advances.</p>
 </div>
 <figure class="roadmap-overview-figure">
  <img src="{{ '/assets/images/micromodular-workflow-deposition-focus.png' | relative_url }}" alt="High-level micromodular electronics roadmap from component fabrication to circuit manufacturing, with deposition step highlighted" loading="lazy">
  <figcaption><strong>High-level roadmap for micromodular electronics.</strong> The highlighted band marks the deposition step between component fabrication and circuit manufacturing. It frames why the substrate screen is judged by placement, crowding, and interconnect-accessible density rather than by final stain appearance alone.</figcaption>
 </figure>
</section>

<section class="artifact-stack flagship-artifacts" aria-label="Micromodular deposition artifacts">
 <article class="artifact-card artifact-card-wide hero-artifact">
  <p class="artifact-label">VIDEO ANALYSIS</p>
  <figure class="artifact-figure">
   <div class="artifact-image-frame frame-wide"><img src="{{ '/assets/images/artifact-microdevice-trajectory-overlay-1400.webp' | relative_url }}" alt="Microdevice trajectory overlay relative to the marked droplet center" loading="lazy"></div>
   <figcaption><strong>Figure 1. Video-derived microdevice trajectories overlaid on a microscope frame.</strong> The droplet center is marked, allowing device motion to be decomposed into radial and tangential components. This converts a qualitative drying/deposition video into a substrate-screening artifact.</figcaption>
  </figure>
  <div class="artifact-meta table-like-meta" aria-label="Run metadata"><span><strong>Solvent</strong> isopropyl alcohol (IPA)</span><span><strong>Metric set</strong> radial velocity, tangential velocity, tracking coverage, edge/center deposition tendency</span><span><strong>Screening method</strong> substrate/backing design-of-experiments (DOE) logic tied to device placement and downstream interconnect feasibility</span><span><strong>Decision output</strong> advance porous-support conditions that preserve drainage without creating edge-heavy crowding</span></div>
 </article>
 <article class="artifact-card artifact-card-wide substrate-artifact">
  <p class="artifact-label">SUBSTRATE SCREEN</p>
  <figure class="artifact-figure">
   <div class="artifact-image-frame frame-wide"><img src="{{ '/assets/images/micromodular-aao-device-comparison.webp' | relative_url }}" alt="AAO substrate baseline, AAO with deposited microdevices, and single micromodular device" loading="lazy"></div>
   <figcaption><strong>Figure 2. AAO substrate and microdevice placement context.</strong> The comparison shows the porous anodic aluminum oxide (AAO) surface, a deposited-device field, and the individual micromodular device form factor. This makes the deposition screen specific to placement on anodic aluminum oxide (AAO)-like supports and connects substrate choice to downstream wiring feasibility.</figcaption>
  </figure>
 </article>
 <article class="artifact-card artifact-card-wide compact-artifact">
  <p class="artifact-label">DEVICE SCALE</p>
  <figure class="artifact-figure">
   <div class="artifact-image-frame frame-microscopy"><img src="{{ '/assets/images/artifact-single-micromodular-device.webp' | relative_url }}" alt="Representative individual micromodular device" loading="lazy"></div>
   <figcaption><strong>Figure 3. Representative micromodular device.</strong> The suspended component is the object that must remain findable, placeable, and accessible to downstream interconnect routing after droplet deposition.</figcaption>
  </figure>
 </article>
 <aside class="artifact-limitation-note"><strong>Scope:</strong> This page now emphasizes the substrate/device screen. The full trajectory dashboard remains on the Droplet Image Analysis Workflows page, where the measurement pipeline is the central artifact.</aside>
</section>

<section class="ownership-callout ownership-callout-large lead-ownership-callout">
 <p>I designed the experiments from scratch: substrate/backing comparisons, top-view and side-view video capture, Python/ImageJ analysis, and placement metrics tied to downstream interconnect feasibility.</p>
</section>

<section class="artifact-panel setup-snapshot">
 <h2>Setup</h2>
 <ul class="snapshot-list">
  <li><strong>System:</strong> isopropyl alcohol (IPA) droplet deposition of suspended microdevices on substrate/backing candidates.</li>
  <li><strong>Inputs varied:</strong> substrate, backing condition, droplet volume, and particle/device loading state.</li>
  <li><strong>Metrics extracted:</strong> normalized radius trace, contact-line regime, edge/center device ratio, qualitative repeatability, and final deposition pattern.</li>
  <li><strong>Current decision:</strong> prioritize porous anodic aluminum oxide (AAO)-like drainage behavior over glass-like evaporation controls.</li>
 </ul>
</section>

<section class="insight-block tone-dark"><p>Boundary conditions controlled the outcome more than the final stain suggested. The deposition problem became a screen for contact-line history, drainage signature, and interconnect-accessible placement.</p></section>

<section class="mini-flow-card"><h2>Screen flow</h2><div class="mini-flow"><span>Prepare substrate/backing</span><b>→</b><span>Deposit droplet</span><b>→</b><span>Extract trace</span><b>→</b><span>Score placement</span><b>→</b><span>Advance AAO-like condition</span></div></section>

## Process levers

Good deposition means uniform areal density, low edge bias, usable placement for downstream interconnects, repeatable droplet behavior, and substrate compatibility with scale-up. Useful placement means lower edge crowding, better center/field distribution, enough local density for downstream interconnect routing, and a substrate/backing condition that can scale beyond brittle AAO coupons.

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

## Next run

<div class="next-iteration-callout">
 <p>The next iteration should set an edge/center ratio and density-uniformity threshold, then compare AAO-like skins against cheaper and less brittle porous supports. The first condition to advance is the porous-support family that preserves drainage without creating edge-heavy crowding.</p>
</div>

## What I owned

<div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Area</th><th>Contribution</th></tr></thead><tbody>
<tr><td>Experimental design</td><td>Substrate/backing comparisons, droplet setup, run-to-run comparison, and early screen logic.</td></tr>
<tr><td>Imaging</td><td>Top-view and side-view capture for footprint, contact-line, and final placement behavior.</td></tr>
<tr><td>Analysis</td><td>Python/OpenCV and ImageJ extraction of normalized contact-line traces, placement metrics, and deposition-screen outputs.</td></tr>
<tr><td>Decision output</td><td>Early gate for whether a substrate/backing condition should advance toward downstream interconnect printing.</td></tr>
</tbody></table></div>

## What changed

<div class="what-changed-block changed-panel">
 <p>This work shifted the project from judging substrates by final visual stains to screening them by video-derived contact-line behavior, drainage/evaporation signatures, and placement metrics tied to interconnect feasibility.</p>
</div>

<div class="case-cta-row two-button-cta">
 <a class="button primary" href="{{ '/projects/printed-interconnect-reliability/' | relative_url }}">Next: Printed Interconnect Reliability →</a>
 <a class="button secondary email-button" href="mailto:{{ site.email }}?subject=Micromodular%20deposition%20case%20file">Email Nathan</a>
</div>
