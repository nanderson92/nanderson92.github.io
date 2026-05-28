---
layout: page
title: Process Simulation and Design
category: Simulation · balances · Georgia Tech
date_range: 2025–present
last_updated: May 2026
noindex: true
metric_chips: '<span>Flowsheet logic</span><span>Assumption tracking</span>'
description: Process simulation work using balances, thermodynamic assumptions, sensitivity checks, and flowsheet decision logic.
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

<section class="artifact-panel evidence-status-card">
 <p class="artifact-label">SUPPORTING WORK</p>
 <h2>Not a featured case file.</h2>
 <p>This page is retained as a supporting work sample, not part of the six public engineering case files. The credible artifact here is the decision structure: basis, assumptions, model selection, sensitivity, and the process choice that the model supports.</p>
</section>

<section class="insight-block tone-dark"><p>A flowsheet is not a final answer. It is a decision aid whose value depends on basis, assumptions, sensitivity, and the design choice it supports.</p></section>

<section class="mini-flow-card"><h2>Decision flow</h2><div class="mini-flow"><span>Basis</span><b>→</b><span>Assumptions</span><b>→</b><span>Model</span><b>→</b><span>Sensitivity</span><b>→</b><span>Design choice</span></div></section>

## Decision variables

<div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Variable</th><th>Why it matters</th><th>Decision use</th></tr></thead><tbody>
<tr><td>Feed composition</td><td>Sets material-balance basis and separation difficulty.</td><td>Defines feasible recovery and purity targets.</td></tr>
<tr><td>Operating temperature/pressure</td><td>Affects phase behavior, duty, and equipment feasibility.</td><td>Compares tradeoffs between energy and separation performance.</td></tr>
<tr><td>Thermodynamic model</td><td>Controls whether predicted vapor-liquid equilibrium (VLE) behavior is physically reasonable.</td><td>Prevents black-box simulation claims.</td></tr>
<tr><td>Recycle/purge logic</td><td>Controls accumulation and steady-state feasibility.</td><td>Determines whether the flowsheet can close.</td></tr>
</tbody></table></div>

## What changed

<div class="what-changed-block changed-panel"><p>The work sharpened how I communicate model outputs: not as a final answer, but as a decision aid tied to basis, assumptions, and sensitivity.</p></div>

<div class="case-cta-row two-button-cta">
 <a class="button primary" href="{{ '/projects/' | relative_url }}">All engineering case files →</a>
 <a class="button secondary email-button" href="mailto:{{ site.email }}?subject=Process%20simulation%20work">Email Nathan</a>
</div>
