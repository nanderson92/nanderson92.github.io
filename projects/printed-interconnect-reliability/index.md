---
layout: page
title: Printed Interconnect Reliability
category: Reliability · printed electronics · Filler Lab · Georgia Tech
date_range: 2025–present
last_updated: May 2026
prev_title: Micromodular Electronics Deposition
prev_url: /projects/micromodular-deposition/
next_title: Thermocycler Process Automation
next_url: /projects/thermocycler-process-automation/
metric_chips: '<span>Failure logic</span><span>Normalized resistance drift screen</span>'
description: Printed interconnect reliability case file using resistance drift, stress intervals, and failure classes to guide upstream process checks.
subtitle: Printed-line testing reframed as a reliability screen that maps resistance behavior back to upstream process checks.
body_class: case-file-page printed-interconnect-reliability
affiliation: Filler Lab · Georgia Tech
---

<section class="artifact-stack reliability-artifacts" aria-label="Printed interconnect measurement artifacts">
 <article class="artifact-card artifact-card-wide hero-artifact">
  <p class="artifact-label">METHOD</p>
  <figure class="artifact-figure">
   <div class="artifact-image-frame frame-schematic"><img src="{{ '/assets/images/four-point-probe-method.svg' | relative_url }}" alt="Redrawn four-point resistance testing method" loading="lazy"></div>
   <figcaption><strong>Figure 1. Measurement method: four-point resistance testing.</strong> Four-point probe logic separates current sourcing from voltage sensing, reducing contact-resistance artifacts when evaluating printed-line resistance and drift.</figcaption>
  </figure>
 </article>
 <article class="artifact-card artifact-card-wide">
  <p class="artifact-label">DRIFT SCREEN</p>
  <figure class="artifact-figure">
   <div class="artifact-image-frame frame-plot"><img src="{{ '/assets/images/reliability-drift-plot.svg' | relative_url }}" alt="Representative normalized resistance drift screen" loading="lazy"></div>
   <figcaption><strong>Figure 2. Representative normalized resistance drift screen.</strong> Resistance normalized to its initial value as a resistance ratio (R/R₀) separates stable traces, smooth drift, intermittent behavior, and threshold crossings that should trigger upstream process checks.</figcaption>
  </figure>
 </article>
 <article class="artifact-card artifact-card-wide evidence-status-card">
  <p class="artifact-label">EVIDENCE STATUS</p>
  <h2>Public view shows the screen architecture and failure-decision logic.</h2>
  <p>Stress-protocol data and microscope evidence can be discussed separately where appropriate. This public page shows the control-plan structure: what should be measured, how failure classes map upstream, and how normalized resistance drift can reveal process-built vulnerability without exposing full unpublished stress data.</p>
 </article>
</section>

<section class="artifact-panel setup-snapshot">
 <h2>Setup</h2>
 <ul class="snapshot-list">
  <li><strong>System:</strong> printed interconnect lines measured before and after stress intervals.</li>
  <li><strong>Inputs handled:</strong> initial resistance, normalized resistance drift (R/R₀), stress timing, probe/contact state, and physical inspection notes.</li>
  <li><strong>Outputs:</strong> pass, monitor, fail, and artifact classes that point to upstream print, cure, handling, or measurement checks.</li>
 </ul>
</section>

<section class="insight-block tone-dark"><p>A printed line can pass an initial continuity check and still carry process-built vulnerability under stress.</p></section>

<section class="mini-flow-card"><h2>Reliability screen flow</h2><div class="mini-flow"><span>Measure initial resistance</span><b>→</b><span>Stress interval</span><b>→</b><span>Measure drift</span><b>→</b><span>Classify</span><b>→</b><span>Check upstream</span></div></section>

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

## Next run

<div class="next-iteration-callout"><p>The next run should pair each resistance trace with a microscope image and stress-protocol row. The engineering decision is whether the observed drift points to print geometry, cure history, material aging, substrate interaction, or a measurement artifact.</p></div>

## What changed

<div class="what-changed-block changed-panel"><p>This work reframed interconnect testing from a time-zero pass/fail check into a reliability screen that can identify process-built vulnerability before full device failure.</p></div>

<section class="related-note-card artifact-panel"><h2>Related note</h2><p><a href="{{ '/notes/' | relative_url }}">Why time-zero continuity is the wrong test for printed lines →</a></p></section>

<div class="case-cta-row two-button-cta">
 <a class="button primary" href="{{ '/projects/thermocycler-process-automation/' | relative_url }}">Next: Thermocycler Process Automation →</a>
 <a class="button secondary email-button" href="mailto:{{ site.email }}?subject=Printed%20interconnect%20case%20file">Email Nathan</a>
</div>
