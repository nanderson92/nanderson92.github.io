---
layout: page
title: Thermocycler Process Automation
category: PID thermal control
tags: Automation · Controls · Diagnostics · Hardware
subtitle: "A biological protocol only works in hardware if the temperature-time trajectory is repeatable: ramp rate, overshoot, settling time, and hold stability are the real product requirements."
---

## Summary

This thermocycler build turned an RT-qPCR-style biological protocol into a controlled temperature-time process. The hard part was not writing PID code; it was making the measured temperature represent what the sample actually experiences.

<div class="role-block">
 <p class="system-label small">MY ROLE</p>
 <p>Prototyped an embedded-controller thermocycler, integrated heating/cooling and sensor feedback, tuned PID behavior, and evaluated ramp rate, overshoot, settling time, and steady-state temperature stability.</p>
</div>

## Problem / motivation

PCR thermal cycling depends on repeatable heating and cooling between temperature setpoints. Poor thermal control creates inconsistent amplification conditions, slower workflows, and unreliable diagnostic performance.

## Representative control artifact

<div class="thermal-artifact proof-artifact-card" aria-label="Temperature versus time profile for thermocycler control">
 <div>
  <p class="system-label small">CONTROL PERFORMANCE VIEW</p>
  <h3>Setpoint tracking and thermal lag</h3>
  <p>The plot format emphasizes the engineering constraints that separate a prototype from a controlled thermal process: sensor placement, ramp-rate limits, overshoot/undershoot, settling time, hold stability, and repeatability across cycles.</p>
 </div>
 <div class="thermal-plot" aria-label="Representative thermal profile with setpoint and measured temperature">
  <span class="plot-axis y">temperature</span>
  <span class="plot-axis x">time</span>
  <b class="setpoint-line"></b>
  <b class="measured-line"></b>
  <em class="annot ramp">ramp rate</em>
  <em class="annot overshoot">overshoot</em>
  <em class="annot hold">hold stability</em>
 </div>
</div>

<div class="hardware-interface-card proof-artifact-card" aria-label="Representative thermocycler hardware interface map">
 <div>
  <p class="system-label small">HARDWARE INTERFACE VIEW</p>
  <h3>Controller → actuator → thermal mass → sensor</h3>
  <p>A representative hardware map makes the control problem concrete: the controller changes actuator output, the thermal block responds with lag, and the sensor closes the loop with imperfect knowledge of actual sample temperature.</p>
 </div>
 <div class="hardware-map" aria-label="Embedded controller thermocycler interface diagram">
  <span>ESP32 / Arduino</span><i></i><span>heater + fan</span><i></i><span>thermal block</span><i></i><span>temperature sensor</span>
 </div>
</div>

## Control-loop schematic

<div class="process-map control-loop-map" aria-label="Representative PID thermal control schematic">
 <div class="process-map-stage"><p>SETPOINT</p><span>denaturation</span><span>annealing</span><span>extension</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage"><p>PID</p><span>error</span><span>gain tuning</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage"><p>ACTUATION</p><span>heater</span><span>cooling fan</span></div>
 <div class="process-map-arrow" aria-hidden="true">→</div>
 <div class="process-map-stage decision-stage"><p>FEEDBACK</p><span>sensor signal vs. sample temperature estimate</span></div>
</div>

## What did not work at first

The first control problem looked like a software problem, but the limiting issue was physical: sensor placement, thermal lag, and heat transfer through the block. Better tuning helped only after the hardware response was treated as part of the process.

## Variables studied

| Variable | Why it matters |
|---|---|
| Ramp rate | Determines total cycle time and diagnostic speed. |
| Steady-state error | Determines whether the sample experiences the intended temperature. |
| Overshoot / undershoot | Can damage assay performance or reduce repeatability. |
| Sensor placement | Affects whether measured temperature represents sample temperature. |
| Controller gains | Determine stability, responsiveness, and oscillation behavior. |
| Heating/cooling balance | Sets whether the device can transition quickly without excessive lag. |

## Methods and tools

<div class="two-col">
 <div class="matrix-card"><h3>Hardware / control</h3><p>Embedded controller, temperature sensor feedback, heater/fan actuation, PID tuning, and thermal cycling scripts.</p></div>
 <div class="matrix-card"><h3>Validation</h3><p>Thermal profile logging, ramp-rate calculation, hold stability checks, repeatability checks, and protocol comparison.</p></div>
</div>

<div class="badge-row"><span class="badge">ESP32</span><span class="badge">Arduino</span><span class="badge">PID Control</span><span class="badge">Sensors</span><span class="badge">RT-qPCR</span><span class="badge">Automation</span></div>

## What I’d do next

The next version would measure closer to the actual sample, not just the thermal block. I would also design the controller around the slowest physical response in the system instead of only chasing faster setpoint tracking, because overshoot that looks acceptable on the block can still be bad for the assay.

<div class="case-cta-row">
 <a class="button primary" href="{{ '/projects/' | relative_url }}">View all projects</a>
 <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Download Resume</a>
 <a class="button tertiary" href="mailto:{{ site.email }}">Contact</a>
</div>
