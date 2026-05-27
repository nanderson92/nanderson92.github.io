---
layout: page
title: Thermocycler Process Automation
category: Automation · Mayo Clinic · Rochester, MN
date_range: Summer 2025
metric_chips: '<span>Control prototype</span><span>Thermal validation CTQs</span>'
subtitle: Embedded thermal-control work framed as validation logic for biological protocols.
---

<section class="artifact-panel public-safe-snapshot">
 <h2>The setup</h2>
 <ul class="snapshot-list">
  <li><strong>Controlled variables:</strong> denaturation, annealing, and extension setpoints.</li>
  <li><strong>Logged variables:</strong> measured block temperature versus time.</li>
  <li><strong>CTQs:</strong> ramp rate, overshoot, settling time, hold stability, and cycle-to-cycle repeatability.</li>
  <li><strong>Main lesson:</strong> sensor placement and thermal lag dominated apparent controller performance.</li>
 </ul>
</section>



<section class="insight-block tone-dark"><p>Sensor placement and thermal lag dominated apparent controller performance.</p></section>

<section class="mini-flow-card"><h2>Control-loop sketch</h2><div class="mini-flow"><span>Setpoint</span><b>→</b><span>Controller output</span><b>→</b><span>Thermal block</span><b>→</b><span>Sensor reading</span><b>→</b><span>Protocol decision</span></div></section>

## What I'd do next

<div class="next-iteration-callout"><p>The next iteration should measure closer to the actual sample, not just the thermal block. The engineering decision is whether the controller should be tuned around block temperature or sample-region thermal history, especially when overshoot and settling time disagree.</p></div>

<section class="visual-artifact-grid" aria-label="Visual artifact slots">
 <figure><img src="{{ '/assets/images/thermocycler-profile.svg' | relative_url }}" alt="Thermocycler temperature profile area" loading="lazy"><figcaption>Artifact placeholder — replace with a real temperature-vs-time graph showing setpoint, measured temperature, overshoot, ramp rate, and hold band.</figcaption></figure>
 <figure><img src="{{ '/assets/images/artifact-device-image.svg' | relative_url }}" alt="Thermocycler prototype image area" loading="lazy"><figcaption>Artifact placeholder — replace with a real prototype hardware, thermal-block, sensor-placement, or wiring photo.</figcaption></figure>
 <figure><img src="{{ '/assets/images/artifact-flow-schematic.svg' | relative_url }}" alt="Thermal control schematic area" loading="lazy"><figcaption>Artifact placeholder — replace with a real controller, heater/cooler, sensor, and sample-region thermal-path schematic.</figcaption></figure>
</section>

## Process levers

<div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Metric</th><th>Why it matters</th><th>What it reveals</th></tr></thead><tbody>
<tr><td>Ramp rate</td><td>Determines cycle time.</td><td>Heating/cooling power and thermal coupling.</td></tr>
<tr><td>Overshoot</td><td>Can damage assay conditions.</td><td>Controller tuning and thermal lag.</td></tr>
<tr><td>Hold stability</td><td>Controls reaction consistency.</td><td>Sensor placement and heat distribution.</td></tr>
<tr><td>Cycle repeatability</td><td>Determines protocol reliability.</td><td>System drift and control robustness.</td></tr>
</tbody></table></div>

## What this shifted

<div class="what-changed-block changed-panel"><p>The project taught me to treat temperature control as a validation problem, not just a code/hardware problem. A setpoint is meaningless unless the sample region actually experiences the intended thermal history.</p></div>


<div class="case-cta-row two-button-cta">
 <a class="button primary" href="{{ '/projects/thin-film-semiconductor-research/' | relative_url }}">Next: Semiconductor Materials Exposure →</a>
 <a class="button secondary email-button" href="mailto:{{ site.email }}">Email Nathan</a>
</div>
