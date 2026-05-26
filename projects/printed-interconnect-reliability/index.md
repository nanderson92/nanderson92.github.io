---
layout: page
title: Printed Interconnect Reliability
category: Reliability · process feedback · 2025–present
date_range: 2025–present
tags: Reliability · Printed Electronics · Electrical Test · Failure Analysis
subtitle: "Turning printed-interconnect resistance behavior into pass, monitor, fail, and artifact decisions tied to upstream process checks."
---

<div class="metric-chip-row"><span class="metric-chip"><strong>Failure</strong> logic</span><span class="metric-chip"><strong>R(t)</strong> screen</span></div>

<section class="artifact-gallery" aria-label="Project artifact panels">
 <figure class="casefile-artifact"><img src="{{ '/assets/images/reliability-drift-plot.svg' | relative_url }}" alt="Reliability drift plot"><figcaption>Measurement plot panel: resistance drift and threshold logic.</figcaption></figure>
 <figure class="casefile-artifact"><img src="{{ '/assets/images/artifact-device-image.svg' | relative_url }}" alt="printed interconnect image"><figcaption>Device/image panel: printed interconnect, probe contact, or line-shape image.</figcaption></figure>
 <figure class="casefile-artifact"><img src="{{ '/assets/images/artifact-flow-schematic.svg' | relative_url }}" alt="reliability screen schematic"><figcaption>Flow schematic panel: measure, classify, and check upstream.</figcaption></figure>
</section>

<div class="thesis-box"><h2>Time-zero function and process robustness are not the same thing.</h2><p>Printed lines need a reliability screen that distinguishes good continuity from process-built vulnerability.</p></div>

## Reliability screen skeleton

<svg class="flow-svg six-node-flow" viewBox="0 0 980 180" role="img" aria-label="Six-node reliability screen flow">
 <defs><marker id="arrow-rel" markerWidth="10" markerHeight="10" refX="8" refY="3" orient="auto"><path d="M0,0 L0,6 L9,3 z" fill="#64748b"/></marker></defs>
 <g class="node"><rect x="10" y="52" width="140" height="70" rx="16"/><text x="80" y="84">Measure</text><text x="80" y="106">initial R</text></g>
 <path d="M155 87 H180" marker-end="url(#arrow-rel)"/>
 <g class="node"><rect x="185" y="52" width="140" height="70" rx="16"/><text x="255" y="84">Normalize</text><text x="255" y="106">to baseline</text></g>
 <path d="M330 87 H355" marker-end="url(#arrow-rel)"/>
 <g class="node"><rect x="360" y="52" width="140" height="70" rx="16"/><text x="430" y="84">Stress</text><text x="430" y="106">interval</text></g>
 <path d="M505 87 H530" marker-end="url(#arrow-rel)"/>
 <g class="node"><rect x="535" y="52" width="140" height="70" rx="16"/><text x="605" y="84">Re-measure</text><text x="605" y="106">time points</text></g>
 <path d="M680 87 H705" marker-end="url(#arrow-rel)"/>
 <g class="node"><rect x="710" y="52" width="120" height="70" rx="16"/><text x="770" y="84">Classify</text><text x="770" y="106">trace</text></g>
 <path d="M835 87 H860" marker-end="url(#arrow-rel)"/>
 <g class="node"><rect x="865" y="52" width="105" height="70" rx="16"/><text x="918" y="84">Check</text><text x="918" y="106">upstream</text></g>
</svg>

## Threshold logic

<svg class="matrix-svg" viewBox="0 0 620 300" role="img" aria-label="Pass fail monitor artifact matrix">
 <rect x="20" y="20" width="270" height="115" rx="18" class="pass"/><text x="155" y="70">PASS</text><text x="155" y="100">Stable R(t), no action</text>
 <rect x="330" y="20" width="270" height="115" rx="18" class="monitor"/><text x="465" y="70">MONITOR</text><text x="465" y="100">Smooth upward drift</text>
 <rect x="20" y="165" width="270" height="115" rx="18" class="fail"/><text x="155" y="215">FAIL</text><text x="155" y="245">Open or large jump</text>
 <rect x="330" y="165" width="270" height="115" rx="18" class="artifact"/><text x="465" y="215">ARTIFACT</text><text x="465" y="245">Retest contact issue</text>
</svg>

## Failure-decision table

| Failure class | What it suggests | Upstream process check |
|---|---|---|
| High initial resistance | Poor print continuity, geometry, or cure | Inspect line shape, cure, and deposition continuity |
| Smooth upward drift | Material aging or environmental sensitivity | Check humidity, sintering/cure, and material stability |
| Sudden open circuit | Cracking, delamination, or handling damage | Inspect physical damage and probe history |
| Intermittent readings | Contact artifact or true instability | Separate probe/contact artifact from line failure |

## Measure, classify, check upstream

<svg class="flow-svg labeled-flow" viewBox="0 0 780 170" role="img" aria-label="Measure classify check upstream flow">
 <defs><marker id="arrow-mcu" markerWidth="10" markerHeight="10" refX="8" refY="3" orient="auto"><path d="M0,0 L0,6 L9,3 z" fill="#64748b"/></marker></defs>
 <rect x="30" y="42" width="180" height="82" rx="18"/><text x="120" y="80">Measure</text><text x="120" y="104">R0 and R(t)</text>
 <path d="M220 83 H285" marker-end="url(#arrow-mcu)"/>
 <rect x="295" y="42" width="180" height="82" rx="18"/><text x="385" y="80">Classify</text><text x="385" y="104">pass/monitor/fail</text>
 <path d="M485 83 H550" marker-end="url(#arrow-mcu)"/>
 <rect x="560" y="42" width="190" height="82" rx="18"/><text x="655" y="80">Check upstream</text><text x="655" y="104">print/cure/probe</text>
</svg>

<div class="changed-panel"><h2>What changed because of this</h2><p>This work reframed interconnect testing from a time-zero pass/fail check into a reliability screen that can identify process-built vulnerability before full device failure.</p></div>

<div class="next-panel"><h2>Open questions / next iteration</h2><p>The next iteration is a full control-plan draft: define public-safe thresholds for pass, monitor, fail, and artifact, then validate the classes across three substrate/interconnect conditions.</p></div>

<div class="cta-row bottom-case-cta"><a class="button primary" href="{{ '/projects/thermocycler-process-automation/' | relative_url }}">Next case file →</a><a class="button secondary email-button" href="mailto:{{ site.email }}">Email Nathan</a></div>
