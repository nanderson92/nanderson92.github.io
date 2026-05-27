---
layout: page
title: Micromodular Electronics Deposition
category: Wet processing · printed electronics · Filler Lab · Georgia Tech
date_range: 2025–present
last_updated: May 2026
metric_chips: '<span>Screening framework</span><span>Image-derived droplet quality metrics</span>'
description: Substrate and backing screens for IPA droplet deposition of suspended microdevices, using video-derived droplet quality metrics and placement metrics.
subtitle: Substrate/backing screens for <abbr title="isopropyl alcohol">IPA</abbr> droplet deposition of suspended microdevices before printed interconnect routing.
body_class: case-file-page
---

<section class="artifact-panel setup-snapshot">
 <h2>Setup</h2>
 <ul class="snapshot-list">
  <li><strong>System:</strong> <abbr title="isopropyl alcohol">IPA</abbr> droplet deposition of suspended microdevices on substrate/backing candidates.</li>
  <li><strong>Inputs varied:</strong> substrate, backing condition, droplet volume, and particle/device loading state.</li>
  <li><strong>Metrics extracted:</strong> <abbr title="droplet radius as a function of time, normalized by initial radius">r(t)/r₀</abbr>, contact-line regime, edge/center device ratio, qualitative repeatability, and final deposition pattern.</li>
  <li><strong>Current decision:</strong> prioritize porous <abbr title="anodic aluminum oxide">AAO</abbr>-like drainage conditions over glass-like evaporation controls.</li>
  <li><strong>Next threshold needed:</strong> replicate-backed edge/center ratio plus density uniformity target before interconnect printing.</li>
 </ul>
</section>
<section class="acronym-legend">
 <strong>Notation:</strong> <span><abbr title="isopropyl alcohol">IPA</abbr> = solvent.</span> <span><abbr title="anodic aluminum oxide">AAO</abbr> = porous substrate reference.</span> <span><abbr title="Critical-to-Quality">CTQ</abbr> = measurable requirement the workflow has to deliver.</span>
</section>

<section class="artifact-stack flagship-artifacts" aria-label="Micromodular deposition artifacts">
 <article class="artifact-card artifact-card-wide hero-artifact">
  <p class="artifact-label">VIDEO ANALYSIS</p>
  <figure class="artifact-figure">
   <div class="artifact-image-frame frame-wide"><img src="{{ '/assets/images/artifact-microdevice-trajectory-overlay.png' | relative_url }}" alt="Microdevice trajectory overlay relative to the marked droplet center" loading="lazy"></div>
   <figcaption><strong>Figure 1. Video-derived microdevice trajectories overlaid on a microscope frame.</strong> The droplet center is marked so device motion can be decomposed into radial and tangential components. This converts a qualitative drying/deposition video into a substrate-screening artifact.</figcaption>
  </figure>
  <div class="artifact-meta table-like-meta" aria-label="Representative artifact metadata"><span><strong>Solvent</strong> IPA</span><span><strong>Artifact status</strong> representative run-level analysis</span><span><strong>Output metrics</strong> radial velocity, tangential velocity, tracking coverage, edge/center deposition tendency</span></div>
 </article>
 <article class="artifact-card artifact-card-wide">
  <p class="artifact-label">RUN DASHBOARD</p>
  <figure class="artifact-figure">
   <div class="artifact-image-frame frame-dashboard"><img src="{{ '/assets/images/artifact-group-motion-dashboard.png' | relative_url }}" alt="Group motion dashboard with speed, radial velocity, angular velocity, and tracking coverage" loading="lazy"></div>
   <figcaption><strong>Figure 2. Group motion dashboard extracted from tracked microdevice trajectories.</strong> The dashboard summarizes population speed, radial velocity, angular-velocity tendency, and tracking coverage over time, allowing deposition behavior to be compared across process conditions.</figcaption>
  </figure>
 </article>
 <article class="artifact-card artifact-card-wide compact-artifact">
  <p class="artifact-label">VELOCITY DECOMPOSITION</p>
  <figure class="artifact-figure">
   <div class="artifact-image-frame frame-plot"><img src="{{ '/assets/images/artifact-radial-tangential-velocity.png' | relative_url }}" alt="Radial and tangential velocity decomposition plot" loading="lazy"></div>
   <figcaption><strong>Figure 3. Radial and tangential velocity decomposition.</strong> Positive radial velocity indicates outward transport from the droplet center; tangential velocity captures circumferential motion. The plotted velocity units reflect the available run calibration for this artifact.</figcaption>
  </figure>
 </article>
 <aside class="artifact-limitation-note"><strong>Current status:</strong> These plots represent preliminary run-level analysis. The next engineering step is replicate-backed comparison across substrate/backing conditions using fixed droplet volume, device loading, frame rate, and calibration.</aside>
</section>

<section class="insight-block tone-dark"><p>Boundary conditions controlled the outcome more than the final stain suggested. The deposition problem became a screen for contact-line history, drainage signature, and interconnect-accessible placement.</p></section>

<section class="mini-flow-card"><h2>Screen flow</h2><div class="mini-flow"><span>Prepare substrate/backing</span><b>→</b><span>Deposit droplet</span><b>→</b><span>Extract r(t)</span><b>→</b><span>Score placement</span><b>→</b><span>Pick next condition</span></div></section>

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

## Next run

<div class="next-iteration-callout">
 <p>The next iteration should set a replicate-backed edge/center ratio and density-uniformity threshold, then compare AAO-like skins against cheaper and less brittle porous supports. The engineering decision is whether the substrate can preserve placement while remaining compatible with downstream interconnect routing.</p>
</div>

## What changed

<div class="what-changed-block changed-panel">
 <p>This work shifted the project from judging substrates by final visual stains to screening them by video-derived contact-line behavior, drainage/evaporation signatures, and placement metrics tied to interconnect feasibility.</p>
</div>

<div class="case-cta-row two-button-cta">
 <a class="button primary" href="{{ '/projects/printed-interconnect-reliability/' | relative_url }}">Next: Printed Interconnect Reliability →</a>
 <a class="button secondary email-button" href="mailto:{{ site.email }}">Email Nathan</a>
</div>
