---
layout: page
title: Process Simulation and Design
category: Simulation · balances · Georgia Tech
date_range: 2025–present
metric_chips: '<span>Flowsheet logic</span><span>Assumption tracking</span>'
subtitle: Flowsheets, balances, thermodynamic reasoning, and simulation-backed design decisions.
---

<section class="artifact-panel public-safe-snapshot"><h2>Design objective</h2><p>Process design work becomes useful when assumptions are visible: basis, feed composition, thermodynamic model, recovery target, purity target, energy duty, and the decision a simulation supports.</p></section>

<section class="visual-artifact-grid" aria-label="Visual artifact slots">
 <figure><img src="{{ '/assets/images/artifact-materials-plot.svg' | relative_url }}" alt="Simulation sensitivity plot area" loading="lazy"><figcaption>Plot area for sensitivity, recovery, purity, duty, or operating-condition comparison.</figcaption></figure>
 <figure><img src="{{ '/assets/images/artifact-device-image.svg' | relative_url }}" alt="Process equipment or data image area" loading="lazy"><figcaption>Image area for process equipment, Aspen screenshot crop, or public-safe design artifact.</figcaption></figure>
 <figure><img src="{{ '/assets/images/artifact-simulation-flow.svg' | relative_url }}" alt="Process simulation schematic area" loading="lazy"><figcaption>Schematic area for PFD, balance structure, or unit-operation chain.</figcaption></figure>
</section>

## Decision variables

<div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Variable</th><th>Why it matters</th><th>Decision use</th></tr></thead><tbody>
<tr><td>Feed composition</td><td>Sets material-balance basis and separation difficulty.</td><td>Defines feasible recovery and purity targets.</td></tr>
<tr><td>Operating T/P</td><td>Affects phase behavior, duty, and equipment feasibility.</td><td>Compares tradeoffs between energy and separation performance.</td></tr>
<tr><td>Thermodynamic model</td><td>Controls whether predicted VLE behavior is physically reasonable.</td><td>Prevents black-box simulation claims.</td></tr>
<tr><td>Recycle/purge logic</td><td>Controls accumulation and steady-state feasibility.</td><td>Determines whether the flowsheet can close.</td></tr>
</tbody></table></div>

## What changed because of this

<div class="what-changed-block changed-panel"><p>The work sharpened how I communicate model outputs: not as a final answer, but as a decision aid tied to basis, assumptions, and sensitivity.</p></div>

## Open questions / next iteration

<div class="next-iteration-callout"><p>The next iteration should make each model assumption testable with one sensitivity plot and one decision statement. The engineering decision is which input would change the recommended flowsheet.</p></div>


<div class="case-cta-row two-button-cta">
 <a class="button primary" href="{{ '/projects/' | relative_url }}">Next case file →</a>
 <a class="button secondary email-button" href="mailto:{{ site.email }}">Email Nathan</a>
</div>
