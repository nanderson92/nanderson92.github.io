---
layout: page
title: Thermocycler Process Automation
category: Automation · Mayo Clinic · Rochester, MN
date_range: Summer 2025
metric_chips: '<span>Control prototype</span><span>Thermal validation CTQs</span>'
description: Thermocycler automation case file focused on thermal-control validation, ramp rate, overshoot, settling time, and hold stability.
subtitle: Embedded thermal-control work framed as validation logic for biological protocols.
body_class: case-file-page
---

<section class="artifact-panel setup-snapshot">
 <h2>The setup</h2>
 <ul class="snapshot-list">
  <li><strong>Controlled variables:</strong> denaturation, annealing, and extension setpoints.</li>
  <li><strong>Logged variables:</strong> measured block temperature versus time.</li>
  <li><strong>CTQs:</strong> ramp rate, overshoot, settling time, hold stability, and cycle-to-cycle repeatability.</li>
  <li><strong>Main lesson:</strong> sensor placement and thermal lag dominated apparent controller performance.</li>
 </ul>
</section>
<section class="acronym-legend">
 <strong>Notation:</strong> <span><abbr title="Critical-to-Quality">CTQ</abbr> = measurable requirement the workflow has to deliver.</span> <span><abbr title="Design of Experiments">DOE</abbr> = structured run plan.</span> <span><abbr title="Failure Mode and Effects Analysis">FMEA</abbr> = failure-mode map used to prioritize checks.</span>
</section>

<section class="artifact-stack" aria-label="Thermocycler artifacts">
 <article class="artifact-card artifact-card-hero">
  <span class="artifact-label">Control hardware</span>
  <div class="artifact-image-wrap hardware-wrap"><img class="artifact-image" src="{{ '/assets/images/artifacts/thermocycler-prototype-front.png' | relative_url }}" alt="Prototype thermocycler automation hardware" loading="lazy"></div>
  <h2>Thermal-control prototype</h2>
  <p class="artifact-caption"><strong>Prototype thermocycler hardware.</strong> This artifact integrates enclosure geometry, fan cooling, electronics, and thermal-control logic into a bench-scale automation system.</p>
 </article>
 <div class="artifact-grid two-col-artifacts">
  <article class="artifact-card">
   <span class="artifact-label">Annotated component image</span>
   <div class="artifact-image-wrap hardware-wrap"><img class="artifact-image" src="{{ '/assets/images/artifacts/thermocycler-prototype-annotated.png' | relative_url }}" alt="Annotated thermocycler prototype hardware" loading="lazy"></div>
   <p class="artifact-caption"><strong>Annotated hardware view.</strong> Numbered labels document the physical subsystem layout and should be verified against the final hardware bill of materials before publication.</p>
  </article>
  <article class="artifact-card">
   <span class="artifact-label">Component legend</span>
   <div class="artifact-table-wrap compact-table-wrap"><table class="artifact-table"><thead><tr><th>Visible label</th><th>Component</th></tr></thead><tbody>
    <tr><td>1</td><td>Printed housing / structural base</td></tr>
    <tr><td>2</td><td>Cooling duct or airflow guide</td></tr>
    <tr><td>3</td><td>Rear housing / fan path shroud</td></tr>
    <tr><td>4</td><td>Control board and wiring region</td></tr>
    <tr><td>5</td><td>Thermal input or sample-region component label to verify</td></tr>
    <tr><td>6</td><td>Fan</td></tr>
   </tbody></table></div>
  </article>
 </div>
 <div class="artifact-grid two-col-artifacts">
  <article class="artifact-card code-artifact">
   <span class="artifact-label">Control code</span>
   <div class="artifact-image-wrap code-image-wrap"><img class="artifact-image" src="{{ '/assets/images/artifacts/thermocycler-code-pid-crop.png' | relative_url }}" alt="PID control code excerpt" loading="lazy"></div>
   <p class="artifact-caption"><strong>Control-code excerpt.</strong> PID logic, thermal-state transitions, and profile execution support the claim that the project involved control implementation, not just CAD or assembly.</p>
  </article>
  <article class="artifact-card code-artifact">
   <span class="artifact-label">Display / feedback code</span>
   <div class="artifact-image-wrap code-image-wrap"><img class="artifact-image" src="{{ '/assets/images/artifacts/thermocycler-code-display-crop.png' | relative_url }}" alt="Display and feedback control code excerpt" loading="lazy"></div>
   <p class="artifact-caption"><strong>Display/feedback code excerpt.</strong> The interface code makes state, setpoint, measured temperature, and timing visible during bench operation.</p>
  </article>
 </div>
 <article class="artifact-placeholder-slot full-width-placeholder"><span class="artifact-label">Add setpoint vs. measured-temperature trace</span><p>Final validation figure should show ramp rate, overshoot, settling time, hold stability, and cycle repeatability.</p></article>
</section>

<section class="insight-block tone-dark"><p>Sensor placement and thermal lag dominated apparent controller performance.</p></section>

<section class="mini-flow-card"><h2>Control-loop sketch</h2><div class="mini-flow"><span>Setpoint</span><b>→</b><span>Controller output</span><b>→</b><span>Thermal block</span><b>→</b><span>Sensor reading</span><b>→</b><span>Protocol decision</span></div></section>

## What I'd do next

<div class="next-iteration-callout"><p>The next iteration should measure closer to the actual sample, not just the thermal block. The engineering decision is whether the controller should be tuned around block temperature or sample-region thermal history, especially when overshoot and settling time disagree.</p></div>

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
