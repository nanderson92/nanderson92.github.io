---
layout: page
title: Process Simulation and Design
category: Simulation · balances · Georgia Tech
date_range: 2025–present
metric_chips: '<span>Flowsheet logic</span><span>Assumption tracking</span>'
description: Process simulation case file using balances, thermodynamic assumptions, sensitivity checks, and flowsheet decision logic.
subtitle: Flowsheets, balances, thermodynamic reasoning, and simulation-backed design decisions.
body_class: case-file-page
---

<section class="artifact-panel setup-snapshot">
 <h2>The setup</h2>
 <ul class="snapshot-list">
  <li><strong>System:</strong> course and side-project flowsheets where balances, thermodynamics, and assumptions determine the recommendation.</li>
  <li><strong>Inputs handled:</strong> basis, feed composition, target purity/recovery, operating temperature/pressure, and model choice.</li>
  <li><strong>Outputs:</strong> decision-ready tables, sensitivity checks, and flowsheet logic that makes assumptions visible.</li>
 </ul>
</section>
<section class="acronym-legend">
 <strong>Notation:</strong> <span><abbr title="Critical-to-Quality">CTQ</abbr> = measurable requirement the workflow has to deliver.</span> <span><abbr title="Design of Experiments">DOE</abbr> = structured run plan.</span> <span><abbr title="Failure Mode and Effects Analysis">FMEA</abbr> = failure-mode map used to prioritize checks.</span>
</section>



<section class="artifact-panel setup-snapshot"><h2>What good looks like</h2><p>Process design work becomes useful when assumptions are visible: basis, feed composition, thermodynamic model, recovery target, purity target, energy duty, and the decision a simulation supports.</p></section>



<section class="insight-block tone-dark"><p>A flowsheet is not a final answer. It is a decision aid whose value depends on basis, assumptions, sensitivity, and the design choice it supports.</p></section>

<section class="mini-flow-card"><h2>Decision flow</h2><div class="mini-flow"><span>Basis</span><b>→</b><span>Assumptions</span><b>→</b><span>Model</span><b>→</b><span>Sensitivity</span><b>→</b><span>Design choice</span></div></section>

## What I'd do next

<div class="next-iteration-callout"><p>The next iteration should make each model assumption testable with one sensitivity plot and one decision statement. The engineering decision is which input would change the recommended flowsheet.</p></div>

<section class="visual-artifact-grid" aria-label="Visual artifact slots">
 <figure><img src="{{ '/assets/images/artifact-materials-plot.svg' | relative_url }}" alt="Simulation sensitivity plot area" loading="lazy"><figcaption>Planned evidence slot — add sensitivity, recovery, purity, duty, or operating-condition comparison.</figcaption></figure>
 <figure><img src="{{ '/assets/images/artifact-device-image.svg' | relative_url }}" alt="Process equipment or data image area" loading="lazy"><figcaption>Planned evidence slot — add process-equipment image, Aspen screenshot crop, or design artifact.</figcaption></figure>
 <figure><img src="{{ '/assets/images/artifact-simulation-flow.svg' | relative_url }}" alt="Process simulation schematic area" loading="lazy"><figcaption>Planned evidence slot — add PFD, balance structure, or unit-operation chain.</figcaption></figure>
</section>

<section class="artifact-link-slot">
 <strong>External artifact slot</strong>
 <span>Planned evidence slot — add poster, GitHub notebook, PDF memo, slide, or shareable writeup link when available.</span>
</section>


## Decision variables

<div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Variable</th><th>Why it matters</th><th>Decision use</th></tr></thead><tbody>
<tr><td>Feed composition</td><td>Sets material-balance basis and separation difficulty.</td><td>Defines feasible recovery and purity targets.</td></tr>
<tr><td>Operating T/P</td><td>Affects phase behavior, duty, and equipment feasibility.</td><td>Compares tradeoffs between energy and separation performance.</td></tr>
<tr><td>Thermodynamic model</td><td>Controls whether predicted VLE behavior is physically reasonable.</td><td>Prevents black-box simulation claims.</td></tr>
<tr><td>Recycle/purge logic</td><td>Controls accumulation and steady-state feasibility.</td><td>Determines whether the flowsheet can close.</td></tr>
</tbody></table></div>

## What this shifted

<div class="what-changed-block changed-panel"><p>The work sharpened how I communicate model outputs: not as a final answer, but as a decision aid tied to basis, assumptions, and sensitivity.</p></div>


<div class="case-cta-row two-button-cta">
 <a class="button primary" href="{{ '/projects/micromodular-deposition/' | relative_url }}">Next: Micromodular Electronics Deposition →</a>
 <a class="button secondary email-button" href="mailto:{{ site.email }}">Email Nathan</a>
</div>
