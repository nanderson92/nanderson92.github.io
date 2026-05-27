---
layout: page
title: Thermocycler Process Automation
category: Automation · Mayo Clinic · Rochester, MN
date_range: Summer 2025
last_updated: May 2026
prev_title: Printed Interconnect Reliability
prev_url: /projects/printed-interconnect-reliability/
next_title: Thin-Film Semiconductor Research
next_url: /projects/thin-film-semiconductor-research/
metric_chips: '<span>Control prototype</span><span>Thermal validation <abbr title="Critical-to-Quality">CTQs</abbr></span>'
description: Thermocycler automation case file focused on thermal-control validation, ramp rate, overshoot, settling time, and hold stability.
subtitle: Embedded thermal-control work framed as validation logic for biological protocols.
body_class: case-file-page
---

<section class="artifact-stack thermocycler-artifacts" aria-label="Thermocycler automation artifacts">
 <article class="artifact-card artifact-card-wide hero-artifact">
  <p class="artifact-label">CONTROL HARDWARE</p>
  <figure class="artifact-figure">
   <div class="artifact-image-frame frame-hardware"><img src="{{ '/assets/images/artifact-thermocycler-front.png' | relative_url }}" alt="Prototype thermocycler hardware with enclosure and electronics" loading="lazy"></div>
   <figcaption><strong>Figure 1. Thermal-control prototype.</strong> Prototype thermocycler hardware integrating enclosure geometry, fan cooling, electronics, and thermal-control logic into a bench-scale automation system.</figcaption>
  </figure>
 </article>
 <article class="artifact-card artifact-card-wide">
  <p class="artifact-label">COMPONENT VIEW</p>
  <figure class="artifact-figure">
   <div class="artifact-image-frame frame-hardware"><img src="{{ '/assets/images/artifact-thermocycler-fan-electronics.png' | relative_url }}" alt="Annotated thermocycler prototype component view" loading="lazy"></div>
   <figcaption><strong>Figure 2. Annotated component image.</strong> Hardware view showing the fan path, electronics, and enclosure geometry that made the controller physically testable.</figcaption>
  </figure>
  <div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Label</th><th>Visible component</th><th>Engineering role</th></tr></thead><tbody>
   <tr><td>1</td><td>Printed housing/base</td><td>Mechanical support and repeatable assembly position.</td></tr>
   <tr><td>2</td><td>Side shroud / enclosure</td><td>Airflow control and physical protection.</td></tr>
   <tr><td>3</td><td>Cooling duct / airflow channel</td><td>Directed cooling path for thermal cycling.</td></tr>
   <tr><td>4</td><td>Control board / electronics</td><td>Controller interface for sensing and actuation.</td></tr>
   <tr><td>5</td><td>Top platform / sample-heater area</td><td>Region where thermal history must be validated.</td></tr>
   <tr><td>6</td><td>Fan / cooling path</td><td>Forced-convection cooling input.</td></tr>
  </tbody></table></div>
 </article>
</section>

<section class="artifact-panel setup-snapshot">
 <h2>Setup</h2>
 <ul class="snapshot-list">
  <li><strong>Controlled variables:</strong> denaturation, annealing, and extension setpoints.</li>
  <li><strong>Logged variables:</strong> measured block temperature versus time.</li>
  <li><strong><abbr title="Critical-to-Quality">CTQs</abbr>:</strong> ramp rate, overshoot, settling time, hold stability, and cycle-to-cycle repeatability.</li>
  <li><strong>Main lesson:</strong> sensor placement and thermal lag dominated apparent controller performance.</li>
 </ul>
</section>
<section class="acronym-legend">
 <strong>Notation:</strong> <span><abbr title="Critical-to-Quality">CTQ</abbr> = measurable requirement the workflow has to deliver.</span> <span><abbr title="Proportional-Integral-Derivative">PID</abbr> = feedback-control structure for adjusting heater/cooling output.</span> <span><abbr title="Failure Mode and Effects Analysis">FMEA</abbr> = failure-mode map used to prioritize checks.</span>
</section>

<section class="artifact-grid artifact-grid-two code-artifact-grid readable-code-grid">
 <article class="artifact-card code-artifact-card">
  <p class="artifact-label">CONTROL LOGIC</p>
  <h2>Controller structure</h2>
  <pre><code class="language-python">class PID:
    def update(self, setpoint, measured_temp, dt):
        error = setpoint - measured_temp
        self.integral += error * dt
        derivative = (error - self.previous_error) / dt
        output = Kp*error + Ki*self.integral + Kd*derivative
        self.previous_error = error
        return clamp(output, 0, 100)</code></pre>
  <p>Condensed control logic shows how the project moved beyond assembly into sensing, actuation, and feedback behavior.</p>
 </article>
 <article class="artifact-card code-artifact-card">
  <p class="artifact-label">STATE LOGIC</p>
  <h2>Thermal-state transitions</h2>
  <pre><code class="language-python">PROFILE = [
    {"state": "denature", "target": 95, "hold_s": 30},
    {"state": "anneal",   "target": 55, "hold_s": 30},
    {"state": "extend",   "target": 72, "hold_s": 60},
]

if stable_near_target(measured_temp, target):
    start_hold_timer()
if hold_timer_done():
    advance_to_next_state()</code></pre>
  <p>State logic matters because biological protocols depend on thermal history, not just whether a nominal setpoint was entered.</p>
 </article>
</section>

<section class="artifact-panel evidence-status-card">
 <p class="artifact-label">VALIDATION STATUS</p>
 <h2>Validation criterion</h2>
 <p>The public page does not include a setpoint-versus-measured-temperature trace. The validation claim is therefore limited to control architecture and the criteria that a final trace must answer: ramp rate, overshoot, settling time, hold stability, and cycle repeatability.</p>
</section>

<section class="insight-block tone-dark"><p>Sensor placement and thermal lag dominated apparent controller performance. A setpoint is not validation unless the sample region sees the intended thermal history.</p></section>

<section class="mini-flow-card"><h2>Control-loop sketch</h2><div class="mini-flow"><span>Setpoint</span><b>→</b><span>Controller output</span><b>→</b><span>Thermal block</span><b>→</b><span>Sensor reading</span><b>→</b><span>Protocol decision</span></div></section>

## Process levers

<div class="artifact-table-wrap"><table class="artifact-table"><thead><tr><th>Metric</th><th>Why it matters</th><th>What it reveals</th></tr></thead><tbody>
<tr><td>Ramp rate</td><td>Determines cycle time.</td><td>Heating/cooling power and thermal coupling.</td></tr>
<tr><td>Overshoot</td><td>Can damage assay conditions.</td><td>Controller tuning and thermal lag.</td></tr>
<tr><td>Hold stability</td><td>Controls reaction consistency.</td><td>Sensor placement and heat distribution.</td></tr>
<tr><td>Cycle repeatability</td><td>Determines protocol reliability.</td><td>System drift and control robustness.</td></tr>
</tbody></table></div>

## Next run

<div class="next-iteration-callout"><p>The next iteration should measure closer to the actual sample, not just the thermal block. The engineering decision is whether the controller should be tuned around block temperature or sample-region thermal history, especially when overshoot and settling time disagree.</p></div>

## What changed

<div class="what-changed-block changed-panel"><p>The project taught me to treat temperature control as a validation problem, not just a code/hardware problem. A setpoint is meaningless unless the sample region actually experiences the intended thermal history.</p></div>

<div class="case-cta-row two-button-cta">
 <a class="button primary" href="{{ '/projects/thin-film-semiconductor-research/' | relative_url }}">Next: Thin-Film Semiconductor Research →</a>
 <a class="button secondary email-button" href="mailto:{{ site.email }}?subject=Thermocycler%20case%20file">Email Nathan</a>
</div>
