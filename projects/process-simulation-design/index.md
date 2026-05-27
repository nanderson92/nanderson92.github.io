---
layout: page
title: Process Simulation and Design
category: Simulation · balances · Georgia Tech
date_range: 2025–present
last_updated: May 2026
metric_chips: '<span>Flowsheet logic</span><span>Assumption tracking</span>'
description: Process simulation case file using balances, thermodynamic assumptions, sensitivity checks, and flowsheet decision logic.
subtitle: Flowsheets, balances, thermodynamic reasoning, and simulation-backed design decisions.
body_class: case-file-page
---

<section class="artifact-panel setup-snapshot">
 <h2>Setup</h2>
 <ul class="snapshot-list">
  <li><strong>System:</strong> course and side-project flowsheets where balances, thermodynamics, and assumptions determine the recommendation.</li>
  <li><strong>Inputs handled:</strong> basis, feed composition, target purity/recovery, operating temperature/pressure, and model choice.</li>
  <li><strong>Outputs:</strong> decision-ready tables, sensitivity checks, and flowsheet logic that makes assumptions visible.</li>
 </ul>
</section>
<section class="acronym-legend">
 <strong>Notation:</strong> <span><abbr title="process flow diagram">PFD</abbr> = process flow diagram.</span> <span><abbr title="vapor-liquid equilibrium">VLE</abbr> = vapor-liquid equilibrium.</span> <span><abbr title="Design of Experiments">DOE</abbr> = structured run plan.</span>
</section>

<section class="artifact-card artifact-card-wide hero-artifact">
 <p class="artifact-label">FLOWSHEET LOGIC</p>
 <figure class="artifact-figure">
  <div class="artifact-image-frame frame-schematic"><img src="{{ '/assets/images/artifact-simulation-flow.svg' | relative_url }}" alt="Process simulation flow schematic" loading="lazy"></div>
  <figcaption><strong>Figure 1. Simulation as decision support.</strong> A model becomes useful when the basis, assumptions, sensitivity, and recommended design choice are visible together.</figcaption>
 </figure>
</section>

<section class="insight-block tone-dark"><p>A flowsheet is not a final answer. It is a decision aid whose value depends on basis, assumptions, sensitivity, and the design choice it supports.</p></section>

<section class="mini-flow-card"><h2>Decision flow</h2><div class="mini-flow"><span>Basis</span><b>→</b><span>Assumptions</span><b>→</b><span>Model</span><b>→</b><span>Sensitivity</span><b>→</b><span>Design choice</span></div></section>

## Decision variables

<div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Variable</th><th>Why it matters</th><th>Decision use</th></tr></thead><tbody>
<tr><td>Feed composition</td><td>Sets material-balance basis and separation difficulty.</td><td>Defines feasible recovery and purity targets.</td></tr>
<tr><td>Operating T/P</td><td>Affects phase behavior, duty, and equipment feasibility.</td><td>Compares tradeoffs between energy and separation performance.</td></tr>
<tr><td>Thermodynamic model</td><td>Controls whether predicted <abbr title="vapor-liquid equilibrium">VLE</abbr> behavior is physically reasonable.</td><td>Prevents black-box simulation claims.</td></tr>
<tr><td>Recycle/purge logic</td><td>Controls accumulation and steady-state feasibility.</td><td>Determines whether the flowsheet can close.</td></tr>
</tbody></table></div>

## Next run

<div class="next-iteration-callout"><p>The next iteration should make each model assumption testable with one sensitivity plot and one decision statement. The engineering decision is which input would change the recommended flowsheet.</p></div>

## What changed

<div class="what-changed-block changed-panel"><p>The work sharpened how I communicate model outputs: not as a final answer, but as a decision aid tied to basis, assumptions, and sensitivity.</p></div>

<div class="case-cta-row two-button-cta">
 <a class="button primary" href="{{ '/projects/microencapsulation-process-development/' | relative_url }}">Next: Stem-Cell Microencapsulation →</a>
 <a class="button secondary email-button" href="mailto:{{ site.email }}">Email Nathan</a>
</div>
