---
layout: page
title: Thermocycler Process Automation
category: Automation · diagnostics · Mayo Clinic · Rochester, MN · Summer 2025
date_range: Summer 2025
affiliation: Mayo Clinic · Rochester, MN
tags: Automation · Thermal Control · Embedded Systems · Diagnostics
subtitle: "Thermal-control validation for a biological protocol where setpoint tracking had to be checked against actual temperature-time behavior."
---

<div class="metric-chip-row"><span class="metric-chip"><strong>Control</strong> prototype</span><span class="metric-chip"><strong>CTQ</strong> time series</span></div>

<section class="artifact-gallery" aria-label="Project artifact panels">
 <figure class="casefile-artifact"><img src="{{ '/assets/images/thermocycler-profile.svg' | relative_url }}" alt="Thermocycler temperature profile"><figcaption>Measurement plot panel: temperature profile, ramp, hold, and overshoot.</figcaption></figure>
 <figure class="casefile-artifact"><img src="{{ '/assets/images/artifact-device-image.svg' | relative_url }}" alt="Thermocycler profile panel"><figcaption>Device/image panel: thermocycler or validation setup image slot.</figcaption></figure>
 <figure class="casefile-artifact"><img src="{{ '/assets/images/artifact-flow-schematic.svg' | relative_url }}" alt="thermal-control schematic"><figcaption>Flow schematic panel: setpoint, measured block response, and validation rule.</figcaption></figure>
</section>

<div class="thesis-box"><h2>A setpoint is not validation.</h2><p>Temperature control only matters when the sample region experiences the intended thermal history.</p></div>

<section class="artifact-panel public-safe-snapshot">
 <h2>Prototype validation snapshot</h2>
 <ul class="snapshot-list"><li><strong>Controlled variables:</strong> denaturation, annealing, and extension setpoints.</li><li><strong>Logged variables:</strong> measured block temperature versus time.</li><li><strong>CTQs:</strong> ramp rate, overshoot, settling time, hold stability, and cycle-to-cycle repeatability.</li><li><strong>Main engineering lesson:</strong> sensor placement and thermal lag dominated apparent controller performance.</li></ul>
</section>

## Thermal-control decision table

| Metric | Why it matters | What it reveals |
|---|---|---|
| Ramp rate | Determines cycle time | Heating/cooling power and thermal coupling |
| Overshoot | Can damage assay conditions | Controller tuning and thermal lag |
| Hold stability | Controls reaction consistency | Sensor placement and heat distribution |
| Cycle repeatability | Determines protocol reliability | System drift and control robustness |

<div class="changed-panel"><h2>What changed because of this</h2><p>The project taught me to treat temperature control as a validation problem, not just a code/hardware problem: a setpoint is meaningless unless the sample region actually experiences the intended thermal history.</p></div>

<div class="next-panel"><h2>Open questions / next iteration</h2><p>The next iteration is to separate controller error from measurement error with a defined validation fixture, sensor-placement check, and repeated protocol run. The decision is whether the prototype can hold assay-relevant temperatures consistently enough to justify tighter PID tuning.</p></div>

<div class="cta-row bottom-case-cta"><a class="button primary" href="{{ '/projects/thin-film-semiconductor-research/' | relative_url }}">Next case file →</a><a class="button secondary email-button" href="mailto:{{ site.email }}">Email Nathan</a></div>
