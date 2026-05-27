---
layout: page
title: Printed Interconnect Reliability
category: Reliability · printed electronics · Filler Lab · Georgia Tech
date_range: 2025–present
metric_chips: '<span>Failure logic</span><span>Resistance drift screen</span>'
subtitle: Printed-line testing reframed as a reliability screen that maps resistance behavior back to upstream process checks.
---

<section class="artifact-panel public-safe-snapshot">
 <h2>What good looks like</h2>
 <p>Time-zero continuity is not enough. The screen classifies resistance drift, sudden failure, intermittent readings, and artifact states so printed interconnect data can feed back into printing, curing, handling, and environmental-stress decisions.</p>
</section>



<section class="insight-block"><p>Time-zero continuity is not enough. Reliability data has to classify drift, failure, and artifacts before it can point back to printing or cure decisions.</p></section>

## What I'd do next

<div class="next-iteration-callout"><p>The next iteration should set public-safe pass, monitor, fail, and artifact thresholds, then validate the classification logic across three substrates. The engineering decision is whether failure class can reliably point to a process correction instead of only describing a dead line.</p></div>

<section class="visual-artifact-grid" aria-label="Visual artifact slots">
 <figure><img src="{{ '/assets/images/reliability-drift-plot.svg' | relative_url }}" alt="Resistance drift plot area" loading="lazy"><figcaption>Artifact placeholder — replace with a real normalized resistance-drift and failure-timing plot.</figcaption></figure>
 <figure><img src="{{ '/assets/images/artifact-device-image.svg' | relative_url }}" alt="Printed interconnect image area" loading="lazy"><figcaption>Artifact placeholder — replace with a real printed-line, probe-layout, or device photo.</figcaption></figure>
 <figure><img src="{{ '/assets/images/artifact-flow-schematic.svg' | relative_url }}" alt="Reliability workflow schematic area" loading="lazy"><figcaption>Artifact placeholder — replace with a real stress interval, re-measurement, and classification workflow diagram.</figcaption></figure>
</section>

## Screen flow

<svg class="flow-svg six-node-flow" viewBox="0 0 1200 260" role="img" aria-label="Six-node reliability screen flow diagram">
 <defs><marker id="arrow-rel" markerWidth="12" markerHeight="12" refX="10" refY="6" orient="auto"><path d="M0 0 L12 6 L0 12 Z" fill="#08708b"/></marker></defs>
 <g font-family="Inter, Arial, sans-serif" font-size="17" font-weight="800" fill="#0f172a">
  <rect x="20" y="70" width="160" height="96" rx="20" fill="#fff" stroke="#d8e2e7"/><text x="100" y="112" text-anchor="middle">Measure</text><text x="100" y="138" text-anchor="middle" font-size="13" fill="#64748b">initial R</text>
  <rect x="220" y="70" width="160" height="96" rx="20" fill="#fff" stroke="#d8e2e7"/><text x="300" y="112" text-anchor="middle">Normalize</text><text x="300" y="138" text-anchor="middle" font-size="13" fill="#64748b">to baseline</text>
  <rect x="420" y="70" width="160" height="96" rx="20" fill="#fff" stroke="#d8e2e7"/><text x="500" y="112" text-anchor="middle">Stress</text><text x="500" y="138" text-anchor="middle" font-size="13" fill="#64748b">interval</text>
  <rect x="620" y="70" width="160" height="96" rx="20" fill="#fff" stroke="#d8e2e7"/><text x="700" y="112" text-anchor="middle">Re-measure</text><text x="700" y="138" text-anchor="middle" font-size="13" fill="#64748b">time points</text>
  <rect x="820" y="70" width="160" height="96" rx="20" fill="#fff" stroke="#d8e2e7"/><text x="900" y="112" text-anchor="middle">Classify</text><text x="900" y="138" text-anchor="middle" font-size="13" fill="#64748b">state</text>
  <rect x="1020" y="70" width="160" height="96" rx="20" fill="#fff" stroke="#d8e2e7"/><text x="1100" y="112" text-anchor="middle">Check</text><text x="1100" y="138" text-anchor="middle" font-size="13" fill="#64748b">upstream</text>
 </g>
 <g stroke="#08708b" stroke-width="4" marker-end="url(#arrow-rel)">
  <line x1="180" y1="118" x2="212" y2="118"/><line x1="380" y1="118" x2="412" y2="118"/><line x1="580" y1="118" x2="612" y2="118"/><line x1="780" y1="118" x2="812" y2="118"/><line x1="980" y1="118" x2="1012" y2="118"/>
 </g>
</svg>

## Classification matrix

<svg class="matrix-svg" viewBox="0 0 900 520" role="img" aria-label="Pass monitor fail artifact matrix">
 <rect width="900" height="520" rx="28" fill="#f8fbfc"/>
 <g font-family="Inter, Arial, sans-serif">
  <rect x="70" y="70" width="350" height="160" rx="22" fill="#eef8f1" stroke="#8fc9a0"/><text x="245" y="130" text-anchor="middle" fill="#0f172a" font-size="30" font-weight="800">PASS</text><text x="245" y="170" text-anchor="middle" fill="#334155" font-size="18">stable after stress</text>
  <rect x="480" y="70" width="350" height="160" rx="22" fill="#fff7df" stroke="#d4a72c"/><text x="655" y="130" text-anchor="middle" fill="#0f172a" font-size="30" font-weight="800">MONITOR</text><text x="655" y="170" text-anchor="middle" fill="#334155" font-size="18">drift before threshold</text>
  <rect x="70" y="290" width="350" height="160" rx="22" fill="#fff4f0" stroke="#d48171"/><text x="245" y="350" text-anchor="middle" fill="#0f172a" font-size="30" font-weight="800">FAIL</text><text x="245" y="390" text-anchor="middle" fill="#334155" font-size="18">open, crack, or high R</text>
  <rect x="480" y="290" width="350" height="160" rx="22" fill="#eef2f7" stroke="#94a3b8"/><text x="655" y="350" text-anchor="middle" fill="#0f172a" font-size="30" font-weight="800">ARTIFACT</text><text x="655" y="390" text-anchor="middle" fill="#334155" font-size="18">retest probe/contact</text>
 </g>
</svg>

## Failure-decision table

<div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Failure class</th><th>What it suggests</th><th>Upstream process check</th></tr></thead><tbody>
<tr><td>High initial resistance</td><td>Poor print continuity, geometry, or cure.</td><td>Inspect line shape, cure condition, deposition continuity, and probe contact.</td></tr>
<tr><td>Smooth upward drift</td><td>Material aging or environmental sensitivity.</td><td>Check humidity exposure, sintering/cure history, and material stability.</td></tr>
<tr><td>Sudden open circuit</td><td>Cracking, delamination, or handling damage.</td><td>Inspect physical damage, probe history, and handling steps.</td></tr>
<tr><td>Intermittent readings</td><td>Contact artifact or true instability.</td><td>Separate probe/contact artifact from line failure by retesting and imaging.</td></tr>
</tbody></table></div>

## Measurement-to-action flow

<svg class="flow-svg labeled-flow" viewBox="0 0 1000 260" role="img" aria-label="Measure classify check upstream flow">
 <defs><marker id="arrow-measure" markerWidth="12" markerHeight="12" refX="10" refY="6" orient="auto"><path d="M0 0 L12 6 L0 12 Z" fill="#08708b"/></marker></defs>
 <g font-family="Inter, Arial, sans-serif">
  <rect x="60" y="62" width="240" height="130" rx="26" fill="#fff" stroke="#d8e2e7"/><text x="180" y="116" text-anchor="middle" font-size="28" font-weight="800" fill="#0f172a">Measure</text><text x="180" y="150" text-anchor="middle" font-size="16" fill="#64748b">R, drift, timing</text>
  <rect x="380" y="62" width="240" height="130" rx="26" fill="#fff" stroke="#d8e2e7"/><text x="500" y="116" text-anchor="middle" font-size="28" font-weight="800" fill="#0f172a">Classify</text><text x="500" y="150" text-anchor="middle" font-size="16" fill="#64748b">pass / monitor / fail / artifact</text>
  <rect x="700" y="62" width="240" height="130" rx="26" fill="#fff" stroke="#d8e2e7"/><text x="820" y="116" text-anchor="middle" font-size="28" font-weight="800" fill="#0f172a">Check upstream</text><text x="820" y="150" text-anchor="middle" font-size="16" fill="#64748b">print, cure, stress, contact</text>
  <line x1="300" y1="127" x2="370" y2="127" stroke="#08708b" stroke-width="5" marker-end="url(#arrow-measure)"/><line x1="620" y1="127" x2="690" y2="127" stroke="#08708b" stroke-width="5" marker-end="url(#arrow-measure)"/>
 </g>
</svg>

## What this shifted

<div class="what-changed-block changed-panel"><p>This work reframed interconnect testing from a time-zero pass/fail check into a reliability screen that can identify process-built vulnerability before full device failure.</p></div>


<div class="case-cta-row two-button-cta">
 <a class="button primary" href="{{ '/projects/thermocycler-process-automation/' | relative_url }}">Next: Thermocycler Process Automation →</a>
 <a class="button secondary email-button" href="mailto:{{ site.email }}">Email Nathan</a>
</div>
