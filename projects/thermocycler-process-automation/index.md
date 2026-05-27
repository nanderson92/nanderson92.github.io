---
layout: page
title: Thermocycler Process Automation
category: Automation · Mayo Clinic · Rochester, MN
date_range: Summer 2025
metric_chips: '<span>Control prototype</span><span>Thermal validation <abbr title="Critical-to-Quality">CTQs</abbr></span>'
subtitle: Embedded thermal-control work framed as validation logic for biological protocols.
meta_description: Case file on thermocycler process automation, ramp rate, overshoot, hold stability, thermal lag, and validation CTQs.
---

<section class="artifact-panel setup-panel"><h2>The setup</h2><ul class="snapshot-list"><li><strong>Controlled variables:</strong> denaturation, annealing, and extension setpoints.</li><li><strong>Logged variables:</strong> measured block temperature versus time.</li><li><strong>CTQs:</strong> ramp rate, overshoot, settling time, hold stability, and cycle-to-cycle repeatability.</li></ul></section>

<section class="insight-block dark-section"><p>Sensor placement and thermal lag dominated apparent controller performance.</p></section>

<section class="next-iteration-callout early-next"><h2>What I’d do next</h2><p>Measure closer to the actual sample, not just the thermal block. The decision is whether the controller should be tuned around block temperature or sample-region thermal history, especially when overshoot and settling time disagree.</p></section>

<section class="visual-artifact-grid" aria-label="Artifact placeholders">
 <figure><img src="{{ '/assets/images/thermocycler-profile.svg' | relative_url }}" alt="Chart artifact placeholder" loading="lazy"><figcaption><strong>Artifact placeholder:</strong> replace with the real chart, graph, trace, or distribution.</figcaption></figure>
 <figure><img src="{{ '/assets/images/artifact-device-image.svg' | relative_url }}" alt="Lab or microscopy artifact placeholder" loading="lazy"><figcaption><strong>Artifact placeholder:</strong> replace with the real lab photo, microscopy still, device image, or run image.</figcaption></figure>
 <figure><img src="{{ '/assets/images/artifact-flow-schematic.svg' | relative_url }}" alt="Code, analysis, or process-flow artifact placeholder" loading="lazy"><figcaption><strong>Artifact placeholder:</strong> replace with code snippet, analysis workflow, control plan, or schematic.</figcaption></figure>
</section>

<section class="flow-diagram-card"><h2>Thermal-control loop</h2><svg class="flow-svg" viewBox="0 0 1000 250" role="img" aria-label="Thermal control loop"><defs><marker id="arrow-therm" markerWidth="12" markerHeight="12" refX="10" refY="6" orient="auto"><path d="M0 0 L12 6 L0 12 Z" fill="#0d8eb1"/></marker></defs><g font-family="Inter, Arial"><rect x="60" y="70" width="180" height="95" rx="20" fill="#fff" stroke="#d8e2e7"/><text x="150" y="125" text-anchor="middle" font-size="22" font-weight="800" fill="#0f172a">Setpoint</text><rect x="300" y="70" width="180" height="95" rx="20" fill="#fff" stroke="#d8e2e7"/><text x="390" y="114" text-anchor="middle" font-size="22" font-weight="800" fill="#0f172a">Controller</text><text x="390" y="140" text-anchor="middle" font-size="14" fill="#64748b">tuning</text><rect x="540" y="70" width="180" height="95" rx="20" fill="#fff" stroke="#d8e2e7"/><text x="630" y="114" text-anchor="middle" font-size="22" font-weight="800" fill="#0f172a">Block</text><text x="630" y="140" text-anchor="middle" font-size="14" fill="#64748b">lag + coupling</text><rect x="780" y="70" width="180" height="95" rx="20" fill="#fff8ea" stroke="#f59e0b"/><text x="870" y="114" text-anchor="middle" font-size="22" font-weight="800" fill="#0f172a">Sample</text><text x="870" y="140" text-anchor="middle" font-size="14" fill="#64748b">actual history</text><line x1="240" y1="118" x2="290" y2="118" stroke="#0d8eb1" stroke-width="5" marker-end="url(#arrow-therm)"/><line x1="480" y1="118" x2="530" y2="118" stroke="#0d8eb1" stroke-width="5" marker-end="url(#arrow-therm)"/><line x1="720" y1="118" x2="770" y2="118" stroke="#0d8eb1" stroke-width="5" marker-end="url(#arrow-therm)"/></g></svg></section>

<h2>Process levers</h2><div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Metric</th><th>Why it matters</th><th>What it reveals</th></tr></thead><tbody><tr><td>Ramp rate</td><td>Determines cycle time.</td><td>Heating/cooling power and thermal coupling.</td></tr><tr><td>Overshoot</td><td>Can damage assay conditions.</td><td>Controller tuning and thermal lag.</td></tr><tr><td>Hold stability</td><td>Controls reaction consistency.</td><td>Sensor placement and heat distribution.</td></tr><tr><td>Cycle repeatability</td><td>Determines protocol reliability.</td><td>System drift and control robustness.</td></tr></tbody></table></div>

<section class="what-changed-block changed-panel"><h2>What this shifted</h2><p>The project taught me to treat temperature control as a validation problem, not just a code/hardware problem. A setpoint is meaningless unless the sample region actually experiences the intended thermal history.</p></section>

<div class="case-cta-row two-button-cta"><a class="button primary" href="{{ '/projects/thin-film-semiconductor-research/' | relative_url }}">Next: Semiconductor Materials Exposure →</a><a class="button secondary email-button" href="mailto:{{ site.email }}">Email Nathan</a></div>
