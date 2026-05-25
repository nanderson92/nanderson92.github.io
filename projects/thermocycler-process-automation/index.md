---
layout: page
title: Thermocycler Process Automation
category: Embedded thermal control
tags: PID Control · ESP32 / Arduino · Diagnostics
subtitle: I built thermal cycling hardware around ramp rate, overshoot, settling time, and hold stability.
---

A thermocycler is not just a box that gets hot and cold. It is a temperature-time process: the biology only works if the sample sees the right profile repeatedly enough to trust the readout.

<figure class="wide-figure thermocycler-profile-figure"><img src="{{ '/assets/images/thermocycler-profile.svg' | relative_url }}" alt="Representative thermocycler temperature profile showing setpoint and measured temperature." loading="eager"><figcaption>Representative control artifact: setpoint profile versus measured temperature, with ramp rate, overshoot, and hold stability called out.</figcaption></figure>

## The hard part

The hard part was sensor truth. A controller can report that it hit a setpoint while the sample region is still lagging. Early tuning made the actuator look responsive but created overshoot that would be unacceptable in a biological protocol, so I shifted the metric from “reaches temperature” to “settles predictably and holds.”

## My role

<div class="role-block"><p>I built and tuned the control workflow around embedded hardware, sensor feedback, PID logic, and repeatable thermal cycling. I focused on the behavior that matters for a protocol: ramp rate, overshoot, settling time, and steady-state error.</p></div>

## Control loop

<div class="process-map compact-flow-map" aria-label="Thermocycler control loop"><div class="process-map-stage"><p>SETPOINT</p><span>denaturation</span><span>annealing</span><span>extension</span></div><div class="process-map-arrow">→</div><div class="process-map-stage"><p>PID</p><span>error</span><span>gain</span><span>update</span></div><div class="process-map-arrow">→</div><div class="process-map-stage"><p>ACTUATION</p><span>heater</span><span>thermal mass</span></div><div class="process-map-arrow">→</div><div class="process-map-stage decision-stage"><p>FEEDBACK</p><span>sensor and sample-lag check</span></div></div>

## What I’d do next

If I built the next version, I would validate sample-temperature lag directly instead of trusting only the control sensor. I would also log every cycle automatically so drift, overshoot, and hold stability are visible before the biology gets blamed for a hardware problem.

<div class="case-cta-row"><a class="button primary" href="{{ '/projects/' | relative_url }}">See all projects</a><a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Resume (PDF, 1 page)</a><a class="button tertiary" href="mailto:{{ site.email }}">Contact</a></div>
