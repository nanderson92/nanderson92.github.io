---
layout: page
title: Micromodular Electronics Deposition
category: Wet processing · printed electronics · 2025–present
date_range: 2025–present
affiliation: Filler Lab · Georgia Tech
tags: Semiconductors · Wet Processing · Interfacial Transport · Data
subtitle: "Substrate/backing screening for IPA droplet deposition of suspended microdevices before downstream printed interconnect routing."
---

<div class="metric-chip-row"><span class="metric-chip"><strong>Screening</strong> framework</span><span class="metric-chip"><strong>Image-derived</strong> droplet CTQs</span></div>

<section class="artifact-gallery" aria-label="Project artifact panels">
 <figure class="casefile-artifact"><img src="{{ '/assets/images/artifact-measurement-plot.svg' | relative_url }}" alt="contact-line measurement plot"><figcaption>Measurement plot panel: r(t)/r0 and contact-line regime comparison.</figcaption></figure>
 <figure class="casefile-artifact"><img src="{{ '/assets/images/micromodular-workflow-deposition-focus.png' | relative_url }}" alt="Micromodular workflow with deposition highlighted"><figcaption>Device/process image panel: micromodular workflow with deposition subsystem highlighted.</figcaption></figure>
 <figure class="casefile-artifact"><img src="{{ '/assets/images/artifact-flow-schematic.svg' | relative_url }}" alt="deposition screen schematic"><figcaption>Flow schematic panel: input variables, video extraction, and screening decision.</figcaption></figure>
</section>

<div class="thesis-box promoted-thesis-box">
 <h2>Useful placement is a CTQ, not a final-photo aesthetic.</h2>
 <p>The screening workflow identifies substrate/backing conditions that reduce edge crowding while preserving interconnect-accessible placement.</p>
</div>

<blockquote class="ownership-callout">Experimental ownership: selected substrates and backing conditions, set up top-view and side-view video capture, wrote Python/OpenCV and ImageJ workflows, then converted droplet behavior into placement metrics.</blockquote>

<section class="artifact-panel public-safe-snapshot" aria-label="Public-safe experiment snapshot">
 <h2>Public-safe experiment snapshot</h2>
 <ul class="snapshot-list">
  <li><strong>System:</strong> IPA droplet deposition of suspended microdevices on substrate/backing candidates.</li>
  <li><strong>Inputs varied:</strong> substrate, backing condition, droplet volume, and particle/device loading state.</li>
  <li><strong>Metrics extracted:</strong> r(t)/r0, contact-line regime, edge/center device ratio, qualitative repeatability, and final deposition pattern.</li>
  <li><strong>Current decision:</strong> prioritize porous AAO-like drainage conditions over glass-like evaporation controls.</li>
  <li><strong>Next threshold needed:</strong> replicate-backed edge/center ratio and density-uniformity target before interconnect printing.</li>
 </ul>
</section>

## Decision framework

<div class="decision-grid two-col">
 <div class="callout decision-pass"><h3>Candidate passes early screen if</h3><ol><li>Contact-line history can be classified from video.</li><li>Edge/center device ratio improves relative to glass-like evaporation control.</li><li>Device density remains high enough for downstream interconnect routing.</li><li>Pattern repeats across replicate droplets.</li><li>Substrate/backing condition is physically scalable beyond brittle AAO.</li></ol></div>
 <div class="callout decision-fail"><h3>Candidate fails if</h3><ul><li>Fast liquid removal still creates edge-heavy crowding.</li><li>Droplet footprint becomes too small or irregular for routing.</li><li>Device rafts or pins unpredictably.</li><li>Metric extraction cannot distinguish mechanism from artifact.</li></ul></div>
</div>

## My role

| Area | Contribution |
|---|---|
| Experimental design | Substrate/backing comparisons, droplet setup, run-to-run screen definition. |
| Imaging | Top-view and side-view capture for spreading, imbibition, and deposition behavior. |
| Analysis | Python/OpenCV and ImageJ extraction of contact-line and deposition metrics. |
| Decision output | Screening logic for substrate candidates before interconnect printing. |

## Defining useful placement

Useful placement means lower edge crowding, stronger center/field distribution, enough local density for downstream interconnect routing, a repeatable final pattern, and substrate compatibility with scale-up.

<div class="changed-panel">
 <h2>What changed because of this</h2>
 <p>This work shifted the project from judging substrates by final visual stains to screening them by video-derived contact-line behavior, drainage/evaporation signatures, and placement metrics tied to downstream interconnect feasibility.</p>
</div>

<div class="next-panel">
 <h2>Open questions / next iteration</h2>
 <p>The next iteration is a replicate-backed screen that fixes droplet volume, loading state, and analysis thresholds while comparing AAO-like skins against cheaper or less brittle candidates. The decision rule should identify when a surface preserves routing-accessible density without creating rim crowding.</p>
</div>

<div class="cta-row bottom-case-cta"><a class="button primary" href="{{ '/projects/microencapsulation-process-development/' | relative_url }}">Next case file →</a><a class="button secondary email-button" href="mailto:{{ site.email }}">Email Nathan</a></div>
