---
layout: page
title: Thermocycler Process Automation
category: Automation · Mayo Clinic · Rochester, MN
date_range: Summer 2025
last_updated: May 2026
prev_title: Printed Interconnect Reliability
prev_url: /projects/printed-interconnect-reliability/
next_title: Thin-Film Characterization-to-Process Logic
next_url: /projects/thin-film-semiconductor-research/
metric_chips: '<span>ESP32/Arduino</span><span>PID thermal control</span><span>Nanoliter qPCR</span>'
description: ESP32/Arduino thermocycler automation case file for nanoliter qPCR, PID thermal control, ramp rate, overshoot, settling time, and hold stability.
subtitle: ESP32/Arduino-controlled thermocycling automation for nanoliter qPCR, focused on whether the sample region sees the intended thermal history.
body_class: case-file-page thermocycler-process-automation
affiliation: Mayo Clinic · Rochester, MN
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

<section class="ownership-callout ownership-callout-large lead-ownership-callout">
 <p><strong>What I owned:</strong> ESP32/Arduino control-logic implementation, thermal-state sequencing, hardware integration support, and validation criteria for ramp rate, overshoot, hold stability, and cycle repeatability.</p>
 <p class="ownership-metric"><strong>Quantified context:</strong> the controller structure organizes three polymerase chain reaction (PCR) temperature stages and four validation targets before final sample-region temperature verification.</p>
</section>

<section class="artifact-panel setup-snapshot">
 <h2>Setup</h2>
 <p><strong>Sensor placement and thermal lag dominated apparent controller performance.</strong> This thermocycler work supported biological PCR: denaturation, annealing, and extension temperature setpoints repeated across cycles, where actual sample-region temperature determines whether the protocol works.</p>
 <ul class="snapshot-list">
  <li><strong>Controlled variables:</strong> denaturation, annealing, and extension setpoints.</li>
  <li><strong>Logged variables:</strong> measured block temperature versus time.</li>
  <li><strong>Critical-to-quality metrics:</strong> ramp rate, overshoot, settling time, hold stability, and cycle-to-cycle repeatability.</li>
  <li><strong>Main lesson:</strong> sensor placement and thermal lag dominated apparent controller performance.</li>
 </ul>
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
  <p>Proportional-integral-derivative (PID) controller excerpt for converting temperature error into heater/cooling output.</p>
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
  <p>Thermal-state machine excerpt for denaturation, annealing, and extension cycles.</p>
 </article>
</section>

<section class="artifact-panel evidence-status-card validation-target-card">
 <p class="artifact-label">VALIDATION TARGET</p>
 <div class="validation-target-grid">
  <div>
   <h2>Setpoint vs. measured-temperature trace</h2>
   <p>Validation is judged by ramp rate, overshoot, settling time, hold stability, and cycle repeatability. The ESP32/Arduino control code matters because it has to produce the intended thermal history at the nanoliter sample region.</p>
  </div>
  <figure>
   <img src="{{ '/assets/images/thermocycler-profile.svg' | relative_url }}" alt="Representative setpoint versus measured temperature profile" loading="lazy">
   <figcaption>Representative validation target for the final trace.</figcaption>
  </figure>
 </div>
</section>

<section class="insight-block tone-dark"><p>Sensor placement and thermal lag dominated apparent controller performance. The sample region, not the nominal setpoint, is the temperature history that matters.</p></section>

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

<div class="what-changed-block changed-panel"><p>The project taught me to treat temperature control as a validation problem, not just a code/hardware problem. Controller behavior only matters when it produces the intended thermal history at the sample region.</p></div>

<div class="case-cta-row two-button-cta">
 <a class="button primary" href="{{ '/projects/thin-film-semiconductor-research/' | relative_url }}">Next: Thin-Film Characterization-to-Process Logic →</a>
 <a class="button secondary email-button" href="mailto:{{ site.email }}?subject=Thermocycler%20case%20file">Email Nathan</a>
</div>
