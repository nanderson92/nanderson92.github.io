---
layout: page
title: Process Simulation and Design
category: Simulation · balances · Georgia Tech
date_range: 2025–present
metric_chips: '<span>Flowsheet logic</span><span>Assumption tracking</span>'
subtitle: Flowsheets, balances, thermodynamic reasoning, and simulation-backed design decisions.
meta_description: Case file on process simulation, material balances, thermodynamics, assumptions, and decision-useful flowsheet design.
---

<section class="artifact-panel setup-panel"><h2>The setup</h2><p>Process design work becomes useful when assumptions are visible: basis, feed composition, thermodynamic model, recovery target, purity target, energy duty, and the decision a simulation supports.</p></section>
<section class="insight-block dark-section"><p>Simulation is not an answer until the assumptions and decision sensitivity are visible.</p></section>
<section class="next-iteration-callout early-next"><h2>What I’d do next</h2><p>Make each model assumption testable with one sensitivity plot and one decision statement. The decision is which input would change the recommended flowsheet.</p></section>
<section class="visual-artifact-grid" aria-label="Artifact placeholders">
 <figure><img src="{{ '/assets/images/artifact-materials-plot.svg' | relative_url }}" alt="Chart artifact placeholder" loading="lazy"><figcaption><strong>Artifact placeholder:</strong> replace with the real chart, graph, trace, or distribution.</figcaption></figure>
 <figure><img src="{{ '/assets/images/artifact-device-image.svg' | relative_url }}" alt="Lab or microscopy artifact placeholder" loading="lazy"><figcaption><strong>Artifact placeholder:</strong> replace with the real lab photo, microscopy still, device image, or run image.</figcaption></figure>
 <figure><img src="{{ '/assets/images/artifact-simulation-flow.svg' | relative_url }}" alt="Code, analysis, or process-flow artifact placeholder" loading="lazy"><figcaption><strong>Artifact placeholder:</strong> replace with code snippet, analysis workflow, control plan, or schematic.</figcaption></figure>
</section>
<h2>Process levers</h2><div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Variable</th><th>Why it matters</th><th>Decision use</th></tr></thead><tbody><tr><td>Feed composition</td><td>Sets material-balance basis and separation difficulty.</td><td>Defines feasible recovery and purity targets.</td></tr><tr><td>Operating T/P</td><td>Affects phase behavior, duty, and equipment feasibility.</td><td>Compares tradeoffs between energy and separation performance.</td></tr><tr><td>Thermodynamic model</td><td>Controls whether predicted VLE behavior is physically reasonable.</td><td>Prevents black-box simulation claims.</td></tr><tr><td>Recycle/purge logic</td><td>Controls accumulation and steady-state feasibility.</td><td>Determines whether the flowsheet can close.</td></tr></tbody></table></div>
<section class="what-changed-block changed-panel"><h2>What this shifted</h2><p>The work made the system easier to judge because the output was tied to a variable, a check, and a next action.</p></section>
<div class="case-cta-row two-button-cta"><a class="button primary" href="{{ '/projects/' | relative_url }}">Next: Engineering Case Files →</a><a class="button secondary email-button" href="mailto:{{ site.email }}">Email Nathan</a></div>
