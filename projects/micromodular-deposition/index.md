---
layout: page
title: Micromodular Electronics Deposition
category: Wet processing · printed electronics · Filler Lab · Georgia Tech
date_range: 2025–present
metric_chips: '<span>Screening framework</span><span>Image-derived droplet quality metrics</span>'
description: Substrate and backing screens for IPA droplet deposition of suspended microdevices, using video-derived droplet quality metrics and placement metrics.
subtitle: Substrate/backing screens for <abbr title="isopropyl alcohol">IPA</abbr> droplet deposition of suspended microdevices before printed interconnect routing.
body_class: case-file-page
last_updated: May 2026
previous_case_title: Stem-Cell Microencapsulation
previous_case_url: /projects/microencapsulation-process-development/
next_case_title: Printed Interconnect Reliability
next_case_url: /projects/printed-interconnect-reliability/
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

<section class="artifact-stack flagship-artifacts" aria-label="Micromodular deposition artifacts">
 <article class="artifact-card artifact-card-wide hero-artifact">
 <p class="artifact-label">VIDEO ANALYSIS</p>
 <figure class="artifact-figure">
 <div class="artifact-image-frame frame-wide"><img src="{{ '/assets/images/artifact-microdevice-trajectory-overlay.png' | relative_url }}" alt="Microdevice trajectory overlay relative to the marked droplet center" loading="lazy"></div>
 <figcaption><strong>Figure 1. Video-derived microdevice trajectories overlaid on a microscope frame.</strong> The droplet center is marked, allowing device motion to be decomposed into radial and tangential components. This converts a qualitative drying/deposition video into a substrate-screening artifact.</figcaption>
 </figure>
 <div class="artifact-meta table-like-meta" aria-label="Run metadata"><span><strong>Solvent</strong> <abbr title="isopropyl alcohol">IPA</abbr></span><span><strong>Droplet volume</strong> held constant within each comparison set</span><span><strong>Substrate/backing</strong> recorded by run condition</span><span><strong>Frame rate</strong> recorded from source video</span><span><strong>Calibration</strong> pixel scale checked before quantitative comparison</span><span><strong>Output metrics</strong> radial velocity, tangential velocity, tracking coverage, edge/center deposition tendency</span></div>
 </article>
 <article class="artifact-card artifact-card-wide">
 <p class="artifact-label">RUN DASHBOARD</p>
 <figure class="artifact-figure">
 <div class="artifact-image-frame frame-dashboard"><img src="{{ '/assets/images/artifact-group-motion-dashboard.png' | relative_url }}" alt="Group motion dashboard with speed, radial velocity, angular velocity, and tracking coverage" loading="lazy"></div>
 <figcaption><strong>Figure 2. Group motion dashboard extracted from tracked microdevice trajectories.</strong> The dashboard summarizes population speed, radial velocity, angular velocity tendency, and tracking coverage over time, allowing deposition behavior to be compared across process conditions.</figcaption>
 </figure>
 </article>
 <article class="artifact-card artifact-card-wide compact-artifact">
 <p class="artifact-label">VELOCITY DECOMPOSITION</p>
 <figure class="artifact-figure">
 <div class="artifact-image-frame frame-plot"><img src="{{ '/assets/images/artifact-radial-tangential-velocity.png' | relative_url }}" alt="Radial and tangential velocity decomposition plot" loading="lazy"></div>
 <figcaption><strong>Figure 3. Radial and tangential velocity decomposition.</strong> Positive radial velocity indicates outward transport from the droplet center; tangential velocity captures circumferential motion. The current public figure is a run-level motion artifact, not a calibrated final process window.</figcaption>
 </figure>
 </article>
 <aside class="artifact-limitation-note"><strong>Current scope:</strong> These plots represent run-level analysis. The next engineering step is replicate-backed comparison across substrate/backing conditions using fixed droplet volume, device loading, frame rate, and calibration.</aside>
</section>

<section class="insight-block tone-dark"><p>Boundary conditions controlled the outcome more than the final stain suggested. The deposition problem became a screen for contact-line history, drainage signature, and interconnect-accessible placement.</p></section>

<section class="mini-flow-card"><h2>Screen flow</h2><div class="mini-flow"><span>Prepare substrate/backing</span><b>→</b><span>Deposit droplet</span><b>→</b><span>Extract r(t)</span><b>→</b><span>Score placement</span><b>→</b><span>Pick next condition</span></div></section>

## What I'd do next

<div class="next-iteration-callout">
 <p>The next iteration should set a replicate-backed edge/center ratio and density-uniformity threshold, then compare AAO-like skins against cheaper and less brittle porous supports. The engineering decision is whether the substrate can preserve placement while remaining compatible with downstream interconnect routing.</p>
</div>





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
